<script>
	export let title, body, link, image;
	let textPos = 1;
	let textPosMD = 2;
	let imgPos = 2;
	let imgPosMD = 1;
	if (image.position == "right") {
		textPos = 2;
		textPosMD = 1;
		imgPos = 1;
		imgPosMD = 2;
	}
</script>

<section class="section mt-5" id="about">
	<div class="container">
		<div class="row align-items-center">
			<div class="col-md-6 order-{textPos} order-md-{textPosMD}">
				<h2 class="section-title">{title}</h2>
				<p>{body}</p>
				<a href={link.url} class="btn-link">{link.title}
					<i class="ti-arrow-right" /></a>
			</div>

			<div class="col-md-6 order-{imgPos} order-md-{imgPosMD} mb-4 mb-md-0">
				<div>
					<img src="assets/{image.url}" class="img-fluid" alt={image.alt} />
				</div>
			</div>
		</div>
	</div>
</section>

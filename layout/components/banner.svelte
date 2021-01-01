<script>
	export let title, image;
</script>

<section class="section pb-0 mt-5">
	<div class="container">
		<div class="row">
			<div class="col-lg-8 mx-auto text-center">
				<h2 class="section-title">{title}</h2>
			</div>
		</div>
	</div>
	<img
		src="/assets{image.url}"
		class="img-fluid w-100" alt="{image.alt}"/>
</section>

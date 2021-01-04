<script>
	export let title, body, link, image;
</script>

<style>
	.banner {
		padding: 70px 0 50px;
	}
</style>

<section class="banner mt-5" id="hero">
	<div class="container">
		<div class="row">
			<div class="col-lg-10 mx-auto text-center">
				<h1 class="mb-3">{title}</h1>
				<p class="mb-4">{body}</p>
				<div><a href={link.url} class="btn btn-primary">{link.title}</a></div>
				<img
					src="/assets{image}"
					class="img-fluid mt-5"
					width="750px"
					alt="two persons looking at websites" />
			</div>
		</div>
	</div>
</section>

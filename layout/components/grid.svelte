<script>
	export let title, items;
</script>

<style>
	.section-title {
		margin-bottom: 30px;
	}
	.feature-card {
		border-radius: 10px;
		padding: 20px;
		transition: 0.2s ease;
		background-color: #fff;
	}
	.shadow,
	.feature-card:hover,
	.btn:hover,
	.btn:active,
	.btn:focus {
		box-shadow: 0 12px 24px -6px rgba(45, 67, 121, 0.1) !important;
	}
	.feature-card i {
		font-size: 30px;
		color: #0aa8a7;
		display: inline-block;
	}
</style>

<section class="section bg-light mt-5" id="services">
	<div class="container">
		<div class="row justify-content-center">
			<div class="col-12 text-center">
				<h2 class="section-title">{title}</h2>
			</div>
			{#each items as item}
				<div class="col-md-4 col-sm-6 mb-4">
					<div class="feature-card text-center">
						<i class="{item.icon} mb-3" />
						<h4 class="mb-2">{item.title}</h4>
						<p>{item.body}</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>

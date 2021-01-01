<script>
	export let title, items;
</script>

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

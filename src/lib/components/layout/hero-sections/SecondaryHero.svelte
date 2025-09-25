<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";

	let {
		title,
		subtitle,
		imageSrc = "https://www.unc.mn/image-placeholder.svg",
		...rest
	}: {
		title: string;
		subtitle: string;
		imageSrc: string;
		[key: string]: any;
	} = $props();
</script>

<header class="border-b border-gray-100 dark:border-gray-900 bg-white dark:bg-gray-950" {...rest}>
	<div class="text-title3 section-px container mx-auto">
		<div class="py-24 lg:py-32 grid gap-16 items-center">
			<!-- Mission-driven content -->
			<div class="text-center max-w-4xl mx-auto space-y-6">
				<h1 class="text-4xl lg:text-6xl font-bold text-gray-900 dark:text-white tracking-tight leading-tight">
					{title}
				</h1>
				<p class="text-lg lg:text-xl text-gray-600 dark:text-gray-300 max-w-2xl mx-auto font-medium leading-relaxed">
					{subtitle}
				</p>
				<!-- Mission statement -->
				<div class="pt-8 max-w-3xl mx-auto">
					<p class="text-base text-gray-700 dark:text-gray-400 leading-relaxed">
						Operations leaders at growing startups waste 40+ hours weekly wrestling with disconnected tools and manual processes. We exist to give those hours back—not through another band-aid solution, but by reverse-engineering how work actually flows and automating what matters most.
					</p>
				</div>
			</div>
			
			<!-- Hero image -->
			<div class="aspect-video overflow-clip rounded-xl bg-gray-100 dark:bg-gray-800 shadow-lg max-w-5xl mx-auto">
				<img
					class="h-full w-full object-cover"
					src={imageSrc}
					alt="Operations team collaborating in a modern workspace"
				/>
			</div>
		</div>
	</div>
</header>

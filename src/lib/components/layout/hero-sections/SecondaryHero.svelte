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

<header class="border-b border-border bg-background" {...rest}>
	<div class="section-px container mx-auto">
		<div class="section-py grid gap-16 items-center">
			<!-- Mission-driven content -->
			<div class="text-center max-w-4xl mx-auto space-y-6">
				<h1 class="text-display font-bold text-foreground tracking-tight leading-tight transition-all duration-300 hover:scale-[1.01]">
					{title}
				</h1>
				<p class="text-title3 text-muted-foreground max-w-2xl mx-auto font-medium leading-relaxed">
					{subtitle}
				</p>
				<!-- Mission statement -->
				<div class="pt-8 max-w-3xl mx-auto">
					<p class="text-body text-foreground/80 leading-relaxed">
						Operations leaders at growing startups waste 40+ hours weekly wrestling with disconnected tools and manual processes. We exist to give those hours back—not through another band-aid solution, but by reverse-engineering how work actually flows and automating what matters most.
					</p>
				</div>
			</div>
			
			<!-- Hero image -->
			<div class="aspect-video overflow-clip bg-card max-w-5xl mx-auto group transition-all duration-500 hover:scale-[1.02]" style="border-radius: var(--radius-xl);">
				<img
					class="h-full w-full object-cover transition-all duration-500 group-hover:scale-105"
					src={imageSrc}
					alt="Operations team collaborating in a modern workspace"
				/>
			</div>
		</div>
	</div>
</header>

<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Forensic precision",
			description: "We reverse-engineer your actual workflows, not what you think they should be. Our approach uncovers the hidden inefficiencies that drain 40+ hours from your team weekly."
		},
		{
			title: "Deployment excellence",
			description: "Borrowing from Palantir's proven methodology, we configure your automation in under an hour through screenshare sessions. No complex setup, no learning curves."
		},
		{
			title: "Community-driven growth",
			description: "We grow through the startup ops community because great operations leaders know other great operations leaders. Word travels fast when you deliver 75% overhead reduction."
		}
	];
</script>

<SecondaryHero
	title="Work smarter, not longer"
	subtitle="Bring clarity to how work really gets done"
	imageSrc="/generated/image-a-group-of-diverse-professionals-gathere.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We started in 2018 with a simple goal: make helpful tech that people actually need. While many chase profits, we chose to do things differently.",
		"Beyond making good products, we care about doing the right thing, being kind to our planet, and making sure everyone can use what we build. That's our compass.",
		"From day one, we've asked ourselves: 'Does this actually help people?' This question gets us through tough calls and shapes who we are. We're playing the long game here.",
		"We think about how our work affects real people's lives. We build tech that brings people together, keeps your information safe, and treats everyone fairly. When we stick to these basics, good things happen."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Meet our founder."
	subtitle="Leading the charge in workflow automation."
	stakeholders={[
		{
			name: "Keith Fearon",
			position: "Founder & CEO",
			bio: "Reverse-engineering enterprise workflows to deliver 75% operational overhead reduction for growing startups.",
			image: "/generated/image-professional-ceo-headshot-portrait-busin.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to reclaim your time?"
	subtitle="75% overhead reduction starts here"
	description="Stop wasting 40+ hours weekly on manual workflows. Join operations leaders at growing startups who've automated their processes in under an hour."
	imageSrc="/generated/image-an-operations-manager-sits-at-a-tidy-des.webp"
/>

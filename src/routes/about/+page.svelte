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
			description: "We reverse-engineer how your team actually works—not theoretical processes or wishful thinking. By analyzing real software usage patterns, we uncover the repetitive tasks that consume 40+ hours of your team's time each week."
		},
		{
			title: "Deployment excellence",
			description: "Built on Palantir-inspired deployment methodology, simplified for startups. One screenshare session, one hour of your time, and your first automation goes live. No training manuals, no configuration headaches."
		},
		{
			title: "Community-driven growth",
			description: "We expand through the startup operations community, where trust spreads through Slack channels and peer recommendations. When you consistently deliver 75% overhead reduction, word travels fast among ops professionals."
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
	title="Meet our founder"
	subtitle="Leading the charge in workflow automation"
	stakeholders={[
		{
			name: "Keith Fearon",
			position: "Founder & CEO",
			bio: "Reverse-engineering enterprise workflows to deliver 75% operational overhead reduction for growing startups.",
			image: "/generated/image-professional-ceo-headshot-portrait-of-a-.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Stop drowning in manual workflows"
	subtitle="Join operations leaders reclaiming 40+ hours weekly"
	description="One screenshare session. One hour of your time. 75% less operational overhead. No complex setup, no learning curves—just proven workflow automation that scales with your growing startup."
	imageSrc="/generated/image-an-operations-manager-celebrating-at-a-m.webp"
/>

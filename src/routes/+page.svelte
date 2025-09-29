<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="Automate the work you didn't sign up for"
	subtitle="Set up workflows in minutes. No specialists needed."
	imageSrc="/generated/image-a-professional-operations-manager-stands.webp"
	centered={false}
/>
<LogoScroller 
	label="Trusted by operations leaders" 
	logoUrls={[
		'https://cdn.brandfetch.io/notion.so/w/400/h/400/logo',
		'https://cdn.brandfetch.io/airtable.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/canva.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/typeform.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="What we do"
	text="Mundane delivers 75% reduction in operational overhead by reverse-engineering actual workflows from your existing enterprise software. We serve operations leaders at growing startups who waste 40+ hours weekly on manual workflows between disconnected tools. Our approach combines enterprise-grade deployment methodology with startup-friendly setup sessions that configure automation in under an hour."
/>

<Testimonials
	testimonials={[
		{
			name: "Carmen Rodriguez",
			position: "VP of Operations",
			company: "Growth Labs",
			quote:
				"Mundane eliminated 42 hours of manual work weekly from our customer onboarding process. What used to take our team 3 days now happens automatically in 45 minutes. We've saved $180K in operational costs this year alone.",
			image: "/generated/image-professional-headshot-of-a-confident-his.webp"
		},
		{
			name: "Marcus Thompson",
			position: "Head of Operations",
			company: "Velocity Dynamics",
			quote:
				"Before Mundane, our data sync between Salesforce and HubSpot broke constantly, risking major deals. Now our revenue pipeline runs flawlessly 24/7. We prevented $2M in lost opportunities and cut our ops hiring needs in half.",
			image: "/generated/image-professional-headshot-of-a-confident-bla.webp"
		},
		{
			name: "Priya Chen",
			position: "Director of Operations",
			company: "Scale Ventures",
			quote:
				"The screenshare setup session delivered exactly what they promised—our entire invoice-to-payment workflow was automated in 52 minutes. We're processing 300% more transactions with the same team size.",
			image: "/generated/image-professional-headshot-of-a-confident-asi.webp"
		}
	]}
/>

<Features
	title="No more duct-taped workflows"
	subtitle="Stop juggling tools and spreadsheets. Mundane automates the busywork between your systems—without the complexity."
	features={[
		{
			title: "Workflow forensics",
			description: "We reverse-engineer how your team actually works across tools like Notion, Asana, and GDrive. No process mapping or guesswork required."
		},
		{
			title: "One-hour setup",
			description: "Share your screen and we'll configure your first automation in under an hour. Skip the endless setup flows of traditional tools."
		},
		{
			title: "75% overhead reduction", 
			description: "Cut 40+ hours of manual work weekly by automating recurring tasks without writing rules from scratch."
		},
		{
			title: "Auto-detection technology",
			description: "Our platform identifies repetitive workflows and builds automations based on real usage patterns. No coding or consultants needed."
		},
		{
			title: "Startup-focused scaling",
			description: "Make operations scale without headcount by enforcing processes that grow with your team—built for first ops hires, not automation experts."
		},
		{
			title: "Palantir-style deployment",
			description: "Enterprise-grade deployment methodology simplified for startups. Trusted by ops professionals who need reliability without complexity."
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />

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
			title: "Engineering excellence",
			description: "Building robust, scalable systems that eliminate deployment failures and streamline complex workflows into intuitive interfaces."
		},
		{
			title: "Developer-first approach",
			description: "Understanding the technical challenges engineering teams face and crafting solutions that integrate seamlessly into existing workflows."
		},
		{
			title: "Operational efficiency",
			description: "Reducing the 40% of time teams waste on debugging deployments, enabling faster feature delivery and sustainable growth."
		}
	];
</script>

<SecondaryHero
	generating
	title="Solving world hunger"
	subtitle="one step at a time"
	imageSrc="https://www.unc.mn/image-placeholder.svg"
/>

<!-- Story Section -->
<Story
	generating
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
	title="Leadership."
	subtitle="Driving innovation in inventory management."
	stakeholders={[
		{
			name: "Fabrizio Soldano",
			position: "Founder & CEO",
			bio: "Passionate about simplifying complex workflows and empowering engineering teams to ship faster.",
			image: "/generated/image-professional-headshot-of-a-male-founder-.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Stop debugging deployments"
	subtitle="Start shipping features weekly"
	description="Join engineering managers at fast-growing SaaS companies who've reclaimed 40% of their time and transformed their deployment process from a bottleneck into a competitive advantage."
	imageSrc="/generated/image-a-professional-engineering-manager-stand.webp"
/>

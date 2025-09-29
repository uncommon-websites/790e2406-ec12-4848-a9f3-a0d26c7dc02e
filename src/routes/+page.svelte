<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";

	// Icons
	import IconActivity from "~icons/lucide/activity";
	import IconShield from "~icons/lucide/shield";
	import IconRotateCcw from "~icons/lucide/rotate-ccw";
	import IconGitBranch from "~icons/lucide/git-branch";
	import IconBarChart3 from "~icons/lucide/bar-chart-3";
	import IconTrendingUp from "~icons/lucide/trending-up";
</script>

<Hero
	title="Build faster. Ship without the stress."
	subtitle="Track changes, catch bugs, and fix failures."
	imageSrc="/generated/image-a-diverse-group-of-professional-engineer.webp"
	centered={false}
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/stripe.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/linear.app/w/400/h/400/logo',
		'https://cdn.brandfetch.io/vercel.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/notion.so/w/400/h/400/logo'
	]}
/>

<Summary
	title="Simple insights for complex systems"
	text="Stop spending 40% of your week debugging failed deployments. Our platform gives engineering managers clear, reliable insight into what's breaking — and why — so teams can spend more time shipping features, not fixing builds.

Modern devops stacks are powerful, but complex. We simplify them into intuitive dashboards that surface the right signals at the right time — no digging through logs or endless Slack threads required."
/>

<Testimonials
	testimonials={[
		{
			name: "Priya Chen",
			position: "VP of Engineering",
			company: "StreamlineIO",
			quote:
				"We went from 12-hour deployment cycles to 45 minutes. Our team now ships features weekly instead of monthly, and deployment failures dropped from 40% to under 3%. This saved us $180K in developer time last quarter alone.",
			image: "/generated/image-professional-headshot-of-a-confident-asi.webp"
		},
		{
			name: "Marcus Thompson",
			position: "Engineering Manager",
			company: "VelocityTech",
			quote:
				"Before, our team spent 60% of their time debugging production issues. Now it's down to 15%. We eliminated weekend emergency calls and reduced our mean time to recovery from 4 hours to 18 minutes. My engineers are finally building features instead of fighting fires.",
			image: "/generated/image-professional-headshot-of-an-african-amer.webp"
		},
		{
			name: "Isabella Rodriguez",
			position: "Senior Engineering Manager",
			company: "ScalePoint",
			quote:
				"The automated rollback system prevented three major incidents that would have cost us $300K in SLA penalties. Our confidence in deployments went from 20% to 95%, and we're now shipping 3x faster with zero production anxiety.",
			image: "/generated/image-professional-headshot-of-a-hispanic-woma.webp"
		}
	]}
/>

<Features
	title="Ship features faster, debug less"
	subtitle="Everything you need to eliminate deployment failures and accelerate your release cycles"
	features={[
		{
			title: "Real-time deployment tracking",
			description: "Monitor every deployment stage with instant alerts that catch issues before they impact users. Never lose sleep over silent failures again.",
			icon: IconActivity
		},
		{
			title: "Intelligent error prevention",
			description: "AI-powered analysis identifies potential deployment risks before they happen. Reduce debugging time by 75% and ship with confidence.",
			icon: IconShield
		},
		{
			title: "One-click rollback safety",
			description: "Instantly revert problematic deployments with zero downtime. Your users stay happy while you fix issues without pressure.",
			icon: IconRotateCcw
		},
		{
			title: "Automated workflow orchestration",
			description: "Connect your entire toolchain with smart automation that handles complex inventory flows. Focus on building features, not managing processes.",
			icon: IconGitBranch
		},
		{
			title: "Performance insights dashboard",
			description: "Track deployment success rates, time-to-recovery metrics, and team velocity in one beautiful interface. Make data-driven decisions effortlessly.",
			icon: IconBarChart3
		},
		{
			title: "Scale without breaking",
			description: "Built for teams shipping weekly to thousands of users. Our infrastructure grows with you, maintaining reliability at any scale.",
			icon: IconTrendingUp
		}
	]}
/>
<AboutTeaser />
<CallToAction
	title="Ship faster. Debug less."
	subtitle="Start free trial"
	description="Engineers lose 40% of their time chasing deployment issues. Our platform removes the guesswork—so your team can get back to building."
	imageSrc="/generated/image-a-cheerful-engineering-manager-in-a-mode.webp"
	callsToAction={[
		{
			href: "/get-started",
			label: "Start free trial",
			variant: "primary"
		},
		{
			href: "/contact",
			label: "Talk to sales",
			variant: "secondary"
		}
	]}
/>

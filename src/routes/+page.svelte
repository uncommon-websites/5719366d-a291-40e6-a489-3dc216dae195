<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero centered={true} />
<LogoScroller 
	label="Trusted by leading investment firms"
	logoUrls={[
		'https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/a16z.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/kleinerperkins.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/generalcatalyst.com/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	generating
	testimonials={[
		{
			name: "Jane Smith",
			position: "CTO",
			company: "Tech Innovations",
			quote:
				"Their cutting-edge automation boosted our productivity by 35%.\nThe intuitive interface reduced training time and improved team adoption.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "John Doe",
			position: "Director of Operations",
			company: "Global Solutions",
			quote:
				"Their robust security protocols gave us confidence in handling sensitive data.\nThe 24/7 support team resolved issues within hours, not days.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sarah Johnson",
			position: "Product Manager",
			company: "Future Systems",
			quote:
				"The scalable platform grew seamlessly with our business needs.\nTheir customization options allowed us to tailor solutions perfectly to our workflows.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	title="AI-powered due diligence at scale"
	subtitle="Transform how your team analyzes investment opportunities with domain-trained AI agents"
	features={[
		{
			title: "Intelligent deal analysis",
			description:
				"Domain-trained AI agents automatically extract and analyze critical data points from pitch decks, financials, and market reports. Stop spending hours on manual data extraction and focus on high-value decision making."
		},
		{
			title: "Seamless data ingestion",
			description:
				"Connect to any data source instantly—from CRM systems to financial databases—and watch as our platform automatically structures and validates information. No more hunting through scattered documents or incomplete data sets."
		},
		{
			title: "Real-time risk assessment",
			description:
				"Get instant risk scores and detailed assessment reports the moment you upload deal documents. Our AI identifies potential red flags and investment opportunities faster than traditional manual review processes."
		},
		{
			title: "Portfolio intelligence",
			description:
				"Track performance patterns across your entire portfolio with AI-powered insights that surface hidden correlations and predict outcomes. Make data-driven decisions with confidence and clarity."
		},
		{
			title: "Market benchmarking",
			description:
				"Compare deals against comprehensive market data and similar transactions in real-time. Access competitive intelligence that positions your investment decisions within the broader market landscape."
		},
		{
			title: "Collaborative workflows",
			description:
				"Enable your entire team to work from a single source of truth with built-in collaboration tools. Share insights, track decisions, and maintain audit trails without compromising data security."
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />

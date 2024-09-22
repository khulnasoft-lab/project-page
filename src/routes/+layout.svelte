<script>
	import './styles.css';
	import Nav from '../components/Nav.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<svelte:head>
	<!-- Website Info -->
	<title>Project | KhulnaSoft Ltd Project Catalog</title>
	<meta name="author" content="KhulnaSoft Ltd" />
	<link rel="canonical" href="https://projects.khulnasoft.com" />
	<meta name="description" content="Project-Page - Free & Open Source apps by KhulnaSoft Ltd" />
	<meta
		name="keywords"
		content="open source, code, privacy, security, linux, self-hosted, projects"
	/>

	<!-- Website Settings -->
	<meta charset="UTF-8" />
	<meta http-equiv="Content-Language" content="en" />
	<meta http-equiv="X-UA-Compatible" content="IE=edge" />
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<meta
		name="viewport"
		content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no, minimal-ui"
	/>

	<!-- Theme colors and site icons -->
	<meta name="theme-color" content="#ec4899" />
	<link rel="icon" href="/favicon.png" type="image/png" />
	<link rel="apple-touch-icon" href="/favicon.png" />

	<!-- Social media tags (Open Graph) -->
	<meta property="og:type" content="website" />
	<meta property="og:title" content="Project-Page | Project Catalog" />
	<meta property="og:description" content="Free & Open Source apps by KhulnaSoft Ltd" />
	<meta property="og:image" content="https://projects.khulnasoft.com/banner.png" />
	<meta property="og:url" content="https://projects.khulnasoft.com" />
	<meta property="og:site_name" content="Project-Page" />

	<!-- Twitter Card Tags -->
	<meta name="twitter:card" content="summary_large_image" />
	<meta name="twitter:title" content="Project-Page | Project Catalog" />
	<meta name="twitter:description" content="Free & Open Source apps by KhulnaSoft Ltd" />
	<meta name="twitter:image" content="https://projects.khulnasoft.com/banner.png" />

	<!-- Hit counter -->
	<script defer data-domain="projects.khulnasoft.com" src="https://no-track.projects.khulnasoft.com/js/script.js"></script>

	<!-- Verification for SEO -->
	<meta name="msvalidate.01" content="3B8A195ACDEB67AAA9AB3BBD8C37E3B6" />

	<!-- Schema.org Markup for Google -->
	<script type="application/ld+json">
		{
			"@context": "http://schema.org",
			"@type": "WebSite",
			"name": "Project-Page",
			"url": "https://projects.khulnasoft.com"
		}
		{
		"@context": "http://schema.org",
		"@type": "Website",
		"headline": "Project-Page | KhulnaSoft Ltd's Project Catalog",
		"image": [
			"https://projects.khulnasoft.com/favicon.png",
			"https://projects.khulnasoft.com/banner.png",
		],
		"datePublished": "2024-01-11T08:00:00+08:00",
		"dateModified": new Date().toString() || "2024-01-11T09:20:00+08:00",
		"author": {
			"@type": "Person",
			"name": "KhulnaSoft Ltd",
			"image": "https://projects.khulnasoft.com/profile.jpg"
		},
		"publisher": {
			"@type": "Organization",
			"name": "Project-Page",
			"logo": { "@type": "ImageObject", "url": "https://projects.khulnasoft.com/favicon.png" }
		},
		"description": "Free and open source apps and services, which respect your privacy",
	}
	</script>
</svelte:head>

<div class="app">
	<Nav />
	<main>
		<slot />
	</main>
	<Footer />
</div>

<style>
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 70rem;
		margin: 0 auto;
		box-sizing: border-box;

		@media (min-width: 1670px) {
			max-width: 85rem;
		}
	}
</style>

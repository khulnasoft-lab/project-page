<script>
	import Hero from '../components/Hero.svelte';
	import ProjectList from '../components/ProjectList.svelte';
	import About from '../components/About.svelte';

	export let data;

	const repos = data.repos || [];
</script>

<svelte:head>
	<title>Project | Home</title>
	<meta name="description" content="Project-Page - Free & Open Source apps by KhulnaSoft Ltd" />
</svelte:head>

<Hero />
<ProjectList projects={repos} />
<About />

<style>
</style>

<script lang="ts">
	import { page } from '$app/state';
	import '../app.css';

	let { children } = $props();

	let scrollY = $state(0);
</script>

<svelte:window bind:scrollY />

<div class="flex min-h-screen flex-col">
	{#snippet link(text: string, href: string)}
		{@const selected = page.url.pathname === href}
		<a
			{href}
			class="border-b font-medium transition hover:text-white
			{selected ? 'text-white' : 'border-transparent text-slate-400'}"
		>
			{text}
		</a>
	{/snippet}

	<div class="content sticky top-0 transition" class:bg-slate-900={scrollY > 0}>
		<nav class="flex items-baseline py-6 text-white">
			<a href="/" class="text-xl font-semibold">Team Durga 3: GT Movies Store</a>

			<div class="ml-auto flex items-baseline gap-8">
				{@render link('Home', '/')}
				{@render link('Team', '/team')}
				{@render link('Project', '/project')}
				{@render link('Demo', '/demo')}
			</div>
		</nav>
	</div>

	<div class="content">
		{@render children()}
	</div>
</div>

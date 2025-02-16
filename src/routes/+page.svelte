<script lang="ts"></script>

<svelte:head>
	<title>Project 1 | Durga 3</title>
</svelte:head>

<div class="py-16">
	<h1 class="text-4xl font-semibold text-white">Project 1: Movies Store</h1>
</div>

<div class="content bg-cyan-950 py-16">
	<h2 class="text-2xl font-semibold text-cyan-50">Objective</h2>

	<p class="mt-4 text-cyan-100">
		Our goal was to create a movie purchasing web app using Django, requested by our client Pranati
		Duvvuri.
	</p>
</div>

<div class="content bg-blue-950 py-16">
	<h2 class="text-2xl font-semibold text-blue-50">What is it?</h2>

	<p class="mt-4 text-blue-100">
		Our project is a way for GT students to rent/buy movies, complete with reviews, order history,
		descriptions, and admin accounts. There were 21 user stories that we had to fulfill, which are
		listed below.
	</p>
</div>

<div class="content bg-indigo-950 py-16">
	<h2 class="text-2xl font-semibold text-indigo-50">User Stories</h2>

	<div class="mt-8 grid gap-2 text-indigo-100 md:grid-cols-3">
		{#snippet story(information: string)}
			<div class="rounded-md bg-indigo-900 p-6">
				<p>{information}</p>
			</div>
		{/snippet}

		{@render story(
			'As a user, I want to see information about the GT Movies Store so I can learn more about the app and its purpose.'
		)}
		{@render story(
			'As a user, I want to register an account so that I can access the GT Movies Store.'
		)}
		{@render story('As a registered user, I want to log in so that I can access my account data.')}
		{@render story(
			'As a registered user, I want to reset my password so that I can regain access to my account if I forget it.'
		)}
		{@render story(
			'As a user, I want to be able to view the list of movies available in the GT Movies Store so I can make my selections.'
		)}
		{@render story('As a user, I want to search movies per title so I can make my selections.')}
		{@render story(
			'As a user, I want to be able to access a shopping cart so I can list all movie items I am willing to purchase.'
		)}
		{@render story(
			'As a user, I want to be able to add one or more items of a movie to my shopping cart so l can purchase them in the future.'
		)}
		{@render story(
			'As a user, I want to create movie reviews so others can use my insights when searching for movies.'
		)}
		{@render story(
			'As a user, I want to be able to remove all movie items from my shopping cart so I can have flexibility on what I purchase or not.'
		)}
		{@render story(
			'As a user, I want to edit my reviews so I have the freedom to change my mind about my reviews.'
		)}
		{@render story(
			'As a user, I want to delete my movie reviews so I have the freedom to change my mind about my reviews.'
		)}
		{@render story(
			'As a user, I want to see the reviews of a movie so I can have information on whether I should purchase a movie or not.'
		)}
		{@render story(
			'As a user, I want to see the details of a movie so I have the information to make my choices.'
		)}
		{@render story(
			'As a user, I want to see a list of my orders so I can track what I have purchased and my expenses.'
		)}
		{@render story(
			'As a user, I want to be able to access the GT Movies Store from any desktop using a web browser, so I can use the app anywhere with an internet connection.'
		)}
		{@render story(
			'As a user, I want the GT Movies Store to feature a responsive Graphical User Interface (GUI) so I can access it through different devices with diverse screen sizes.'
		)}
		{@render story(
			'As an administrator, I want to be able to manage (view, create, update, or delete) users from the GT Movies Store so we can keep information up to date.'
		)}
		{@render story(
			'As an administrator, I want to be able to manage (view, create, update, or delete) movies from the GT Movies Store so we can keep information up to date.'
		)}
		{@render story(
			'As an administrator, I want to be able to manage (create, update, or delete) reviews from the GT Movies Store so we can keep information up to date.'
		)}
		{@render story(
			'As an administrator, I want to be able to manage (create, update, or delete) orders from the GT Movies Store so we can keep information up to date.'
		)}
	</div>
</div>

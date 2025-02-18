<script lang="ts"></script>

<svelte:head>
	<title>Our Project | Durga 3</title>
</svelte:head>

<div class="py-16">
	<h1 class="text-4xl font-semibold text-white">Our Project</h1>

	<p class="mt-4 leading-relaxed text-slate-300">
		Our project is focused on 21 user stories, including <strong
			>movies and descriptions, adding/editing/deleting reviews, adding movies to the cart, ordering
			movies and viewing order history, and managing the web app with an admin account</strong
		>. We used <b>Django</b> and <b>Trello</b> to complete this project. We used Django to create the
		web app, and Trello to plan out which of our user stories to prioritize. Django helped us with creating
		admin accounts to manage the website data.
	</p>
</div>

<div class="content bg-cyan-950 py-16">
	<h2 class="text-3xl font-semibold text-cyan-50">Accounts</h2>

	<div class="mt-8 grid gap-8 text-cyan-100 md:grid-cols-2">
		<div>
			<img src="/project/login.png" alt="" class="w-full rounded-xl" />
			<p class="mt-4">
				Users can log into the website by entering their username and password that they created at
				signup. Incorrect usernames and passwords will prevent the user from logging in.
			</p>
			<p class="mt-4">
				If users don't remember their password, they can choose to reset it with the <i
					>Reset Password</i
				> functionality.
			</p>
		</div>
		<div>
			<img src="/project/signup.png" alt="" class="w-full rounded-xl" />
			<p class="mt-4">
				Users can register with a username and a password. They will be asked to confirm their
				password by typing it a second time.
			</p>
			<p class="mt-4">
				The account creation request will be rejected if the username is already taken, if the
				passwords do not match, or if the password is not strong enough.
			</p>
		</div>
	</div>
</div>

<div class="content bg-blue-950 py-16">
	<h2 class="text-3xl font-semibold text-blue-50">Movies</h2>

	<div class="mt-8 grid gap-8 text-blue-100 md:grid-cols-2">
		<div>
			<img src="/project/list.png" alt="" class="w-full rounded-xl" />
			<p class="mt-4">
				Users can see a list of movies available to purchase on the website, and they have the
				option to click on a movie to view more details.
			</p>
		</div>
		<div>
			<img src="/project/search.png" alt="" class="w-full rounded-xl" />
			<p class="mt-4">
				Users can search for movies that they want to see, narrowing down the list of movies
				displayed on the website.
			</p>
		</div>
	</div>
</div>

<div class="content bg-indigo-950 py-16">
	<h2 class="text-3xl font-semibold text-indigo-50">Details</h2>

	<div class="mt-8 grid gap-4 text-indigo-100 md:grid-cols-3">
		<div>
			<img src="/project/moviedetails.png" alt="" class="w-full rounded-xl" />
			<p class="mt-4">
				When clicking on a movie, users will see a variety of information including a description,
				pricing, and reviews.
			</p>
		</div>
		<div>
			<img src="/project/review.png" alt="" class="w-full rounded-xl" />
			<p class="mt-4">
				Users will have the option to leave a review for a movie, which will be displayed on the
				movie's details page.
			</p>
		</div>
		<div>
			<img src="/project/reviewedit.png" alt="" class="w-full rounded-xl" />
			<p class="mt-4">
				After making a review, users can edit or delete their review if they change their mind.
			</p>
		</div>
	</div>
</div>

<div class="content bg-blue-950 py-16">
	<h2 class="text-3xl font-semibold text-blue-50">Orders</h2>

	<div class="mt-8 grid gap-4 text-blue-100 md:grid-cols-3">
		<div>
			<img src="/project/buy.png" alt="" class="w-full rounded-xl" />
			<p class="mt-4">
				On the movie detail page, users can add a movie to their cart. They can select any quantity
				of the movie they want to purchase.
			</p>
		</div>
		<div>
			<img src="/project/cart.png" alt="" class="w-full rounded-xl" />
			<p class="mt-4">
				In the shopping cart, users can see all the movies they have added to their cart. They can
				choose to remove all movies from the cart or proceed to purchase.
			</p>
		</div>
		<div>
			<img src="/project/orders.png" alt="" class="w-full rounded-xl" />
			<p class="mt-4">
				After purchasing movies, users can view their order history to see what they have purchased
				and how much they have spent.
			</p>
		</div>
	</div>
</div>

<div class="content bg-cyan-950 py-16">
	<h2 class="text-3xl font-semibold text-cyan-50">Process</h2>

	<p class="mt-4">
		The System Sequence Diagram shows the process of a user logging in, viewing and searching
		movies, adding, editing, and deleting reviews, adding movies to the cart, ordering movies, and
		viewing their order history.
	</p>

	<img src="/project/process.png" alt="" class="mt-8 w-full rounded-xl" />
</div>

<style>
	strong,
	b {
		color: var(--color-slate-50);
		font-weight: 600;
	}
</style>

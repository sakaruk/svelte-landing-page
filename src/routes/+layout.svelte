<script>
	const scrollActive = false;
</script>

<header
	class={'fixed top-0 w-full  z-30 bg-white-500 transition-all ' +
		(scrollActive ? ' shadow-md pt-0' : ' pt-4')}
>
	<nav class="max-w-screen-xl px-6 sm:px-8 lg:px-16 mx-auto grid grid-flow-col py-3 sm:py-4">
		<div class="col-start-1 col-end-2 flex items-center">
			<span class="h-8 w-auto">Logo</span>
		</div>
		<ul class="hidden lg:flex col-start-4 col-end-8 text-black-500  items-center">
			<li>
				<a
					class="px-4 py-2 mx-2 cursor-pointer animation-hover inline-block relative text-orange-500 animation-active"
					href="#about"
				>
					About
				</a>
			</li>
			<li>
				<a
					class="px-4 py-2 mx-2 cursor-pointer animation-hover inline-block relative text-black-500 hover:text-orange-500 a"
					href="#feature"
				>
					Feature
				</a>
			</li>
			<li>
				<a
					class="px-4 py-2 mx-2 cursor-pointer animation-hover inline-block relative text-black-500 hover:text-orange-500 a"
					href="#pricing"
				>
					Pricing
				</a>
			</li>
			<li>
				<a
					class="px-4 py-2 mx-2 cursor-pointer animation-hover inline-block relative text-black-500 hover:text-orange-500 a"
					href="#testimonial"
				>
					Testimonial
				</a>
			</li>
		</ul>
		<div class="col-start-10 col-end-12 font-medium flex justify-end items-center">
			<a
				href="/"
				class="text-black-600 mx-2 sm:mx-4 capitalize tracking-wide hover:text-orange-500 transition-all"
			>
				Sign In
			</a>
			<button
				class="font-medium tracking-wide py-2 px-5 sm:px-8 border border-orange-500 text-orange-500 bg-white-500 outline-none rounded-l-full rounded-r-full capitalize hover:bg-orange-500 hover:text-white-500 transition-all hover:shadow-orange "
			>
				Sign Up
			</button>
		</div>
	</nav>
</header>
<slot />
<div class="bg-white-300 pt-44 pb-24">
	<div
		class="max-w-screen-xl w-full mx-auto px-6 sm:px-8 lg:px-16 grid grid-rows-6 sm:grid-rows-1 grid-flow-row sm:grid-flow-col grid-cols-3 sm:grid-cols-12 gap-4"
	>
		<div
			class="row-span-2 sm:col-span-4 col-start-1 col-end-4 sm:col-end-5 flex flex-col items-start "
		>
			<span class="h-8 w-auto mb-6">Logo</span>
			<p class="mb-4">
				<strong class="font-medium">LaslesVPN</strong> is a private virtual network that has unique features
				and has high security.
			</p>
			<div class="flex w-full mt-2 mb-8 -mx-2">
				<div class="mx-2 bg-white-500 rounded-full items-center justify-center flex p-2 shadow-md">
					FB
				</div>
				<div class="mx-2 bg-white-500 rounded-full items-center justify-center flex p-2 shadow-md">
					TW
				</div>
				<div class="mx-2 bg-white-500 rounded-full items-center justify-center flex p-2 shadow-md">
					IG
				</div>
			</div>
			<p class="text-gray-400">©{new Date().getFullYear()} - LaslesVPN</p>
		</div>
		<div class=" row-span-2 sm:col-span-2 sm:col-start-7 sm:col-end-9 flex flex-col">
			<p class="text-black-600 mb-4 font-medium text-lg">Product</p>
			<ul class="text-black-500 ">
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Download</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Pricing</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Locations</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Server</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Countries</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Blog</li>
			</ul>
		</div>
		<div class="row-span-2 sm:col-span-2 sm:col-start-9 sm:col-end-11 flex flex-col">
			<p class="text-black-600 mb-4 font-medium text-lg">Engage</p>
			<ul class="text-black-500">
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">LaslesVPN</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">FAQ</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Tutorials</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">About Us</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Privacy Policy</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Terms of Service</li>
			</ul>
		</div>
		<div class="row-span-2 sm:col-span-2 sm:col-start-11 sm:col-end-13 flex flex-col">
			<p class="text-black-600 mb-4 font-medium text-lg">Earn Money</p>
			<ul class="text-black-500">
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Affiliate</li>
				<li class="my-2 hover:text-orange-500 cursor-pointer transition-all">Become Partner</li>
			</ul>
		</div>
	</div>
</div>

<script>
	import { each } from 'svelte/internal';
	import '../app.css';
	const countWidgets = [
		{
			name: 'Users',
			number: '390',
			icon: '/assets/Icon/heroicons_sm-user.svg'
		},
		{
			name: 'Locations',
			number: '20',
			icon: '/assets/Icon/gridicons_location.svg'
		},
		{
			name: 'Server',
			number: '50',
			icon: '/assets/Icon/bx_bxs-server.svg'
		}
	];

	const features = [
		'Powerfull online protection.',
		'Internet without borders.',
		'Supercharged VPN',
		'No specific time limits.'
	];
</script>

<div class="max-w-screen-xl x-8 xl:px-16 mx-auto" id="about">
	<div class="scroll-animation-wrapper">
		<div
			class="grid grid-flow-row sm:grid-flow-col grid-rows-2 md:grid-rows-1 sm:grid-cols-2 gap-8 py-6 sm:py-16"
		>
			<div class=" flex flex-col justify-center items-start row-start-2 sm:row-start-1">
				<h1 class="text-3xl lg:text-4xl xl:text-5xl font-medium text-black-600 leading-normal">
					Want anything to be easy with <strong>LaslesVPN</strong>.
				</h1>
				<p class="text-black-500 mt-4 mb-6">
					Provide a network for all your needs with ease and fun using LaslesVPN discover
					interesting features from us.
				</p>
				<button>Get Started</button>
			</div>
			<div class="flex w-full">
				<div class="h-full w-full">
					<img src="/assets/Illustration1.png" alt="VPN Illustrasi" width={612} height={383} />
				</div>
			</div>
		</div>
	</div>
	<div class="relative w-full flex">
		<div
			class="scroll-animation-wrapper rounded-lg w-full grid grid-flow-row sm:grid-flow-row grid-cols-1 sm:grid-cols-3 py-9 divide-y-2 sm:divide-y-0 sm:divide-x-2 divide-gray-100 bg-white-500 z-10"
		>
			{#each countWidgets as countWidget}
				<div
					class="flex items-center justify-start sm:justify-center py-4 sm:py-6 w-8/12 px-4 sm:w-auto mx-auto sm:mx-0"
				>
					<div class="flex mx-auto w-40 sm:w-auto">
						<div class="flex items-center justify-center bg-orange-100 w-12 h-12 mr-6 rounded-full">
							<img src={countWidget.icon} alt={countWidget.name} class="h-6 w-6" />
						</div>
						<div class="flex flex-col">
							<p class="text-xl text-black-600 font-bold">
								{countWidget.number}+
							</p>
							<p class="text-lg text-black-500">{countWidget.name}</p>
						</div>
					</div>
				</div>
			{/each}
		</div>
		<div
			class="absolute bg-black-600 opacity-5 w-11/12 roudned-lg h-64 sm:h-48 top-0 mt-8 mx-auto left-0 right-0"
			style="filter: blur(114px);"
		/>
	</div>
</div>

<div class="max-w-screen-xl mt-8 mb-6 sm:mt-14 sm:mb-14 px-6 sm:px-8 lg:px-16 mx-auto" id="feature">
	<div class="grid grid-flow-row sm:grid-flow-col grid-cols-1 sm:grid-cols-2 gap-8 p  y-8 my-12">
		<div class="scroll-animation-wrapper flex w-full justify-end">
			<motion.div class="h-full w-full p-4">
				<img src="/assets/Illustration2.png" alt="VPN Illustrasi" height={414} width={508} />
			</motion.div>
		</div>
		<div class="scroll-animation-wrapper">
			<div class="flex flex-col items-end justify-center ml-auto w-full lg:w-9/12">
				<h3 class="text-3xl lg:text-4xl font-medium leading-relaxed text-black-600">
					We Provide Many Features You Can Use
				</h3>
				<p class="my-2 text-black-500">
					You can explore the features that we provide with fun and have their own functions each
					feature.
				</p>
				<ul class="text-black-500 self-start list-inside ml-8">
					{#each features as feature}
						<li class="relative circle-check custom-list">
							{feature}
						</li>
					{/each}
				</ul>
			</div>
		</div>
	</div>
</div>

<div class="bg-gradient-to-b from-white-300 to-white-500 w-full py-14" id="pricing">
	<div
		class="max-w-screen-xl  px-6 sm:px-8 lg:px-16 mx-auto flex flex-col w-full text-center justify-center"
	>
		<div class="flex flex-col w-full">
			<div class="scroll-animation-wrapper">
				<h3 class="text-2xl sm:text-3xl lg:text-4xl font-medium text-black-600 leading-relaxed">
					Choose Your Plan
				</h3>
				<p class="leading-normal w-10/12 sm:w-7/12 lg:w-6/12 mx-auto my-2 text-center">
					Let's choose the package that is best for you and explore it happily and cheerfully.
				</p>
			</div>
			<div
				class="grid grid-flow-row sm:grid-flow-col grid-cols-1 sm:grid-cols-3 gap-4 lg:gap-12 py-8 lg:py-12 px-6 sm:px-0 lg:px-6"
			>
				<div class="scroll-animation-wrapper flex justify-center">
					<div
						class="flex flex-col justify-center items-center border-2 border-gray-500 rounded-xl py-4 px-6 lg:px-12 xl:px-20"
					>
						<div class="p-4 lg:p-0 mt-6 lg:mt-16">
							<img src="/assets/Free.png" width={145} height={165} alt="Free Plan" />
						</div>
						<p class="text-lg text-black-600 font-medium capitalize my-2 sm:my-7">Free Plan</p>
						<ul
							class="flex flex-col list-inside pl-6 xl:pl-0 items-start justify-start text-left text-black-500 flex-grow"
						>
							<li class="relative check custom-list my-2">Unlimited Bandwitch</li>
							<li class="relative check custom-list my-2">Encrypted Connection</li>
							<li class="relative check custom-list my-2">No Traffic Logs</li>
							<li class="relative check custom-list my-2">Works on All Devices</li>
						</ul>
						<div class="flex flex-col w-full justify-center mb-8 flex-none mt-12">
							<p class="text-2xl text-black-600 text-center mb-4 ">Free</p>
							<button>Select</button>
						</div>
					</div>
				</div>
				<div class="scroll-animation-wrapper flex justify-center">
					<div
						class="flex flex-col justify-center items-center border-2 border-gray-500 rounded-xl py-4 px-6 lg:px-12 xl:px-20"
					>
						<div class="p-4 lg:p-0 mt-6 lg:mt-16">
							<img src="/assets/Standard.png" width={145} height={165} alt="Standard Plan" />
						</div>
						<p class="text-lg text-black-600 font-medium capitalize my-2 sm:my-7">
							Standard Plan{' '}
						</p>
						<ul
							class="flex flex-col list-inside pl-6 xl:pl-0 items-start justify-start text-left text-black-500 flex-grow"
						>
							<li class="relative check custom-list my-2">Unlimited Bandwitch</li>
							<li class="relative check custom-list my-2">Encrypted Connection</li>
							<li class="relative check custom-list my-2">No Traffic Logs</li>
							<li class="relative check custom-list my-2">Works on All Devices</li>
							<li class="relative check custom-list my-2">
								Connect Anyware{' '}
							</li>
						</ul>
						<div class="flex flex-col w-full justify-center mb-8 flex-none mt-12">
							<p class="text-2xl text-black-600 text-center mb-4 ">
								$9 <span class="text-black-500">/ mo</span>
							</p>
							<button>Select</button>
						</div>
					</div>
				</div>
				<div class="scroll-animation-wrapper flex justify-center">
					<div
						class="flex flex-col justify-center items-center border-2 border-gray-500 rounded-xl py-4 px-6 lg:px-12 xl:px-20"
					>
						<div class="p-4 lg:p-0 mt-6 lg:mt-16">
							<img src="/assets/Premium.png" width={145} height={165} alt="Premium Plan" />
						</div>
						<p class="text-lg text-black-600 font-medium capitalize my-2 sm:my-7">
							Premium Plan{' '}
						</p>
						<ul
							class="flex flex-col list-inside pl-6 xl:pl-0 items-start justify-start text-left text-black-500 flex-grow"
						>
							<li class="relative check custom-list my-2">Unlimited Bandwitch</li>
							<li class="relative check custom-list my-2">Encrypted Connection</li>
							<li class="relative check custom-list my-2">No Traffic Logs</li>
							<li class="relative check custom-list my-2">Works on All Devices</li>
							<li class="relative check custom-list my-2">
								Connect Anyware{' '}
							</li>
							<li class="relative check custom-list my-2">
								Get New Features{' '}
							</li>
						</ul>
						<div class="flex flex-col w-full justify-center mb-8 flex-none mt-12">
							<p class="text-2xl text-black-600 text-center mb-4 ">
								$12 <span class="text-black-500">/ mo</span>
							</p>

							<button>Select</button>
						</div>
					</div>
				</div>
			</div>
		</div>
		<div class="flex flex-col w-full my-16">
			<div class="scroll-animation-wrapper">
				<h3
					class="text-2xl sm:text-3xl lg:text-4xl font-medium text-black-600 leading-relaxed w-9/12 sm:w-6/12 lg:w-4/12 mx-auto"
				>
					Huge Global Network of Fast VPN{' '}
				</h3>
				<p class="leading-normal  mx-auto my-2 w-10/12 sm:w-7/12 lg:w-6/12">
					See LaslesVPN everywhere to make it easier for you when you move locations.
				</p>
			</div>
			<div class="scroll-animation-wrapper">
				<div class="py-12 w-full px-8 mt-16">
					<div class="w-full h-auto">Maps</div>
				</div>
			</div>
			<div class="scroll-animation-wrapper">
				<div class="w-full flex justify-evenly items-center mt-4 flex-wrap lg:flex-nowrap">
					<img src="/assets/Icon/amazon.png" class="h-14 w-auto mt-4 lg:mt-2" alt="" />
					<img src="/assets/Icon/netflix.png" class="h-14 w-auto mt-2 lg:mt-0" alt="" />
					<img src="/assets/Icon/reddit.png" class="h-12 w-auto mt-2 lg:mt-0" alt="" />
					<img src="/assets/Icon/discord.png" class="h-14 w-auto mt-2 lg:mt-0" alt="" />
					<img src="/assets/Icon/spotify.png" class="h-12 w-auto mt-2 lg:mt-0" alt="" />
				</div>
			</div>
		</div>
		<div class="flex flex-col w-full my-16" id="testimoni">
			<div class="scroll-animation-wrapper">
				<h3
					class="text-2xl sm:text-3xl lg:text-4xl font-medium text-black-600 leading-normal w-9/12 sm: lg:w-4/12 mx-auto"
				>
					Trusted by Thousands of Happy Customer{' '}
				</h3>
				<p class="leading-normal mx-auto mb-2 mt-4 w-10/12 sm:w-7/12 lg:w-6/12">
					These are the stories of our customers who have joined us with great pleasure when using
					this crazy feature.
				</p>
			</div>
			<div class="scroll-animation-wrapper w-full flex flex-col py-12">
				<div>Testimonials</div>
			</div>
			<div class="scroll-animation-wrapper relative w-full mt-16">
				<div>
					<div
						class="absolute rounded-xl  py-8 sm:py-14 px-6 sm:px-12 lg:px-16 w-full flex flex-col sm:flex-row justify-between items-center z-10 bg-white-500"
					>
						<div class="flex flex-col text-left w-10/12 sm:w-7/12 lg:w-5/12 mb-6 sm:mb-0">
							<h5
								class="text-black-600 text-xl sm:text-2xl lg:text-3xl leading-relaxed font-medium"
							>
								Subscribe Now for <br /> Get Special Features!
							</h5>
							<p>Let's subscribe with us and find the fun.</p>
						</div>
						<button>Get Started</button>
					</div>
					<div
						class="absolute bg-black-600 opacity-5 w-11/12 roudned-lg h-60 sm:h-56 top-0 mt-8 mx-auto left-0 right-0"
						style="filter: blur(114px);"
					/>
				</div>
			</div>
		</div>
	</div>
</div>

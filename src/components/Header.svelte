<script>
	import Logo from '../lib/assets/Button.png';
	import Home from '../lib/assets/Home.png';
	import Explore from '../lib/assets/Explore.png';
	import Learn from '../lib/assets/Learn.png';
	import Post from '../lib/assets/Post.png';
	import { Button } from '$lib/components/ui/button/index.js';
	import * as Avatar from '$lib/components/ui/avatar/index.js';
	import DP from '../lib/assets/DP.png';
	import * as DropdownMenu from '$lib/components/ui/dropdown-menu/index.js';
	import { ChevronDown, LogOut, Settings } from 'lucide-svelte';
</script>

<header
	class="flex sticky top-0 max-w-[1400px] p-4 border-b border-dotted backdrop-filter backdrop-blur justify-between z-50"
>
	<div class="flex items-center">
		<img src={Logo} alt="Duggup Logo" />
	</div>

	<nav class="flex items-center justify-between text-[#4D4D4D] font-normal space-x-8">
		<ul class="flex items-center space-x-8">
			<li>
				<a href="/" class="flex gap-x-2 items-center">
					<img src={Home} alt="Home Icon" />
					Home
				</a>
			</li>
			<li>
				<a href="/" class="flex gap-x-2 items-center">
					<img src={Explore} alt="Explore Icon" />
					Explore
				</a>
			</li>
			<li>
				<a href="/" class="flex gap-x-2 items-center">
					<img src={Learn} alt="Explore Icon" />
					Learn
				</a>
			</li>
			<Button
				class="bg-white text-[#4D4D4D] border border-b-4 border-[#4D4D4D] hover:bg-slate-200 rounded-md gap-x-2 px-4  "
			>
				<img src={Post} alt="Post Icon" />
				Post
			</Button>
			<DropdownMenu.Root class="mt-4">
				<DropdownMenu.Trigger class="flex items-center gap-x-3">
					<Avatar.Root class="border border-[#4D4D4D]">
						<Avatar.Image src={DP} alt="DP Icon" />
						<Avatar.Fallback>DP</Avatar.Fallback>
					</Avatar.Root>
					<p class="text-md">Krishna Kiran</p>
					<ChevronDown class="w-3" />
				</DropdownMenu.Trigger>

				<DropdownMenu.Content class="w-48">
					<DropdownMenu.Group>
						<DropdownMenu.Item class="flex gap-x-4" value="top">
							<Settings class="mr-2 h-4 w-4" />
							<span>Settings</span>
						</DropdownMenu.Item>
						<DropdownMenu.Item class="flex gap-x-4" value="bottom">
							<LogOut class="mr-2 h-4 w-4" />
							<span>Log out</span>
						</DropdownMenu.Item>
					</DropdownMenu.Group>
				</DropdownMenu.Content>
			</DropdownMenu.Root>
		</ul>
	</nav>
</header>

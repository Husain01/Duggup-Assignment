<script>
	import Headshot from '$lib/assets/Headshot.png';
	import * as Avatar from '$lib/components/ui/avatar/index.js';
	import Button from '$lib/components/ui/button/button.svelte';
	import ExternalLink from '$lib/assets/ExternalLink.png';
	import DuggupIcon from '$lib/assets/DuggupIcon.png';
	import HorizontalDot from '$lib/assets/HorizontalDot.png';
	let isFollowing = false;

	function toggleFollow() {
		isFollowing = !isFollowing;
	}
</script>

<div class="flex items-center justify-center pt-12 gap-x-14">
	<div class="flex flex-col flex-wrap max-w-32">
		<Avatar.Root class="border-[5px] border-[#EAEFF5] size-32 z-0">
			<Avatar.Image src={Headshot} alt="DP Icon" class="z-0"/>
			<Avatar.Fallback>DP</Avatar.Fallback>
		</Avatar.Root>
		<h1 class="text-[#4B5C6D] text-2xl font-bold text-center text-wrap pt-2.5">Krishna Kiran</h1>
	</div>
	<div class="flex flex-col gap-y-5">
        <div class="flex justify-between gap-x-20">
            <p class="max-w-prose leading-6">
				Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of
				Engineering. I write hot-takes on building a business, shipping delightful products and
				accelerating product and career growth.
			</p>
            <div class="flex flex-col items-end gap-2">
                <div>
                    <img src={DuggupIcon} alt="" />
                </div>
                <div class="flex flex-col items-end">
                    <p class="font-bold text-base">Duggup</p>
                    <p class="text-xs text-[#7A9299] text-nowrap">Co-Founder and CEO</p>
                </div>
            </div>
        </div>
        <div class="flex justify-between">
            <Button
				on:click={toggleFollow}
				class="bg-white text-[#4D4D4D] hover:bg-[#0066FF] hover:text-white border border-b-4 border-[#4D4D4D] rounded-md gap-x-2 px-4  hover:border-[#0066FF] hover:border-b-[#003A91] cursor-pointer w-fit"
				>{isFollowing ? 'Followed' : 'Follow'}</Button
			>
            <div class="flex gap-4 items-center">
				<a
					href="https://husainbhagat.me"
					class="flex gap-2 items-center text-nowrap"
					target="_blank"
					>My website
					<div>
						<img src={ExternalLink} alt="Link Icon" />
					</div>
				</a>
				<div>
					<img src={HorizontalDot} alt="Menu Icon" />
				</div>
			</div>
        </div>
	</div>
</div>

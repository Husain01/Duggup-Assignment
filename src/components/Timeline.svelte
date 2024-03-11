<script>
	import * as Card from '$lib/components/ui/card';
	import Blog1 from '$lib/assets/Blog1.png';
	import Blog2 from '$lib/assets/Blog2.png';
	import Blog3 from '$lib/assets/Blog3.png';
	import Blog4 from '$lib/assets/Blog4.png';
    import BlogTimeline from '$lib/assets/BlogTimeline.png';
    import ArrowIcon from '$lib/assets/ArrowIcon.svg';
    import RoleTimeline from '$lib/assets/RoleTimeline.svg';
    import DuggupRole from '$lib/assets/DuggupRole.png';
    import BetterUpRole from '$lib/assets/BetterUpRole.png';
</script>

<section class="flex  flex-col pt-6  pl-24">
	<div class="flex items-center gap-x-9">
		<div class="h-72 border-r-4 border-dotted relative flex items-center justify-end w-48">
			<p class="pr-8">Dec 2023</p>
            <img src={BlogTimeline} alt="Blog TimeLine Icon" class="absolute -right-2.5" />
		</div>
		<div>
			<Card.Root class="max-w-80">
				<Card.Header class="p-0 ">
					
						<img src={Blog1} alt="Steve Jobs" class="h-32 object-cover w-full rounded-t-md" />
					
				</Card.Header>
				<Card.Content class="p-6">
					<Card.Title class="line-clamp-2 max-w-prose text-wrap text-sm font-normal "
						>No amount of technology can convert a bad story into a good story.</Card.Title
					>
				</Card.Content>
			</Card.Root>
		</div>
		<div>
			<Card.Root class="max-w-80">
				<Card.Header class="p-0">
						<img src={Blog2} alt="Sam Altman" class="h-32 object-cover w-full rounded-t-md" />
				</Card.Header>
				<Card.Content class="p-6">
					<Card.Title class="line-clamp-2 max-w-prose text-wrap text-sm font-normal "
						>Most people don't have original ideas. Here is how Sam Altman pushes himself to have
						unpopular ideas.</Card.Title
					>
				</Card.Content>
			</Card.Root>
		</div>
	</div>
	<div class="flex items-center gap-x-9">
		<div class="h-40 border-r-4 border-dotted relative flex flex-col items-end justify-center pr-8 w-48">
            <div>
                <img src={DuggupRole} alt="Duggup Icon">
            </div>
			<h3 class="font-bold text-base">Duggup</h3>
            <p class="text-xs text-[#7A9299] pt-1">San Francisco Bay Area</p>
            <p class="text-xs text-[#7A9299] pt-0.5">Joined</p>
            <p class="text-xs text-[#7A9299]">Nov 2023</p>
            <img src={RoleTimeline} alt="Role TimeLine Icon" class="absolute -right-5" />
            <img src={ArrowIcon} alt="Arrow Icon" class="absolute top-0 -right-2.5" />
		</div>
		<div class="max-w-2xl bg-white px-5 py-4 w-full rounded-md">
			<h2 class="font-bold text-xl">Co-Founder and CEO</h2>
            <p class="text-[#7A9299] text-xs pt-1">Full-time · Remote</p>
		</div>
	</div>
	<div class="flex items-center gap-x-9">
		<div class="h-72 border-r-4 border-dotted relative flex items-center justify-end w-48">
			<p class="pr-8">Dec 2023</p>
            <img src={BlogTimeline} alt="Blog TimeLine Icon" class="absolute -right-2.5" />
		</div>
		<div>
			<Card.Root class="max-w-80">
				<Card.Header class="p-0 ">
					
						<img src={Blog3} alt="Steve Jobs" class="h-32 object-cover w-full rounded-t-md" />
					
				</Card.Header>
				<Card.Content class="p-6">
					<Card.Title class="line-clamp-2 max-w-prose text-wrap text-sm font-normal "
						>Startup Lesson I am reflecting. Don't build for the "average person".</Card.Title
					>
				</Card.Content>
			</Card.Root>
		</div>
		<div>
			<Card.Root class="max-w-80">
				<Card.Header class="p-0">
						<img src={Blog4} alt="Sam Altman" class="h-32 object-cover w-full rounded-t-md" />
				</Card.Header>
				<Card.Content class="p-6">
					<Card.Title class="line-clamp-2 max-w-prose text-wrap text-sm font-normal "
						>Your biggest regrets at 80 will be acts of omission.</Card.Title
					>
				</Card.Content>
			</Card.Root>
		</div>
	</div>
    <div class="flex items-center gap-x-9">
		<div class="h-40 border-r-4 border-dotted relative flex flex-col items-end justify-center pr-8 w-48">
            <div>
                <img src={BetterUpRole} alt="BetterUp Icon">
            </div>
			<h3 class="font-bold text-base">BetterUp</h3>
            <p class="text-xs text-[#7A9299] pt-1">San Francisco Bay Area</p>
            <p class="text-xs text-[#7A9299] pt-0.5">Joined</p>
            <p class="text-xs text-[#7A9299]">Sep 2022</p>
            <img src={RoleTimeline} alt="Role TimeLine Icon" class="absolute -right-5" />
            <img src={ArrowIcon} alt="Arrow Icon" class="absolute top-0 -right-2.5" />
		</div>
		<div class="max-w-2xl bg-white px-5 py-4 w-full shadow-[0_1px_2px_0_rgba(219,229,245,0.25)] rounded-md">
			<h2 class="font-bold text-xl">VP Engineering</h2>
            <p class="text-[#7A9299] text-xs pt-1">Full-time</p>
		</div>
	</div>
</section>

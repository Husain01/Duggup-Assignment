<script>
	import Header from '../components/Header.svelte';
	import Profile from '../components/Profile.svelte';
	import Timeline from '../components/Timeline.svelte';
</script>

<main class="flex flex-col max-w-[1400px] w-full mx-auto ">
	<Header />
    <!-- <div class="flex flex-col justify-center w-2/3 mx-auto"> -->
        <Profile />
        <Timeline/>
    <!-- </div> -->
</main>

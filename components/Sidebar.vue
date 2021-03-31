<template>
  <aside
		class="flex flex-col items-center bg-white text-gray-700 shadow h-full">
		<!-- Side Nav Bar-->
		<div class="h-16 flex items-center w-full">
			<!-- Logo Section -->
			<a class="h-6 w-6 mx-auto" href="http://svelte.dev/">
				<img
					class="h-6 w-6 mx-auto"
					src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/Svelte_Logo.svg/512px-Svelte_Logo.svg.png"
					alt="svelte logo" />
			</a>
		</div>
		<ul>

			<li class="hover:bg-green-400">
        <NuxtLink to="/">
          <div
            class="h-16 px-6 flex flex justify-center items-center w-full
            focus:text-orange-500">
            <IconDrive />
          </div>
         </NuxtLink>
			</li>

			<li class="hover:bg-green-400">
        <NuxtLink to="/blog">
          <div
            class="h-16 px-6 flex flex justify-center items-center w-full
            focus:text-orange-500">
            <IconBookmark />
          </div>
        </NuxtLink>
			</li>
		</ul>
	</aside>
</template>

<script>
import IconDrive from './icons/IconDrive';
import IconBookmark from './icons/IconBookmark';

export default {
  components : {
    IconDrive,
    IconBookmark
  }
}
</script>

<style>

</style>
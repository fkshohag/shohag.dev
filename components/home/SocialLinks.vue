<template>
	<div>
		<h2 class="mb-4 text-xs font-semibold uppercase text-gray-400">
			Socials
		</h2>
		<div
			class="flex space-x-4"
		>
			<NuxtLink
				v-for="(link, index) in links"
				:key="link.icon"
				v-motion-pop-visible
				:delay="index*50"
				:to="link.url"
				target="_blank"
				external
				:aria-label="link.name + ' profile'"
				class="hover:text-primary-300 group flex items-end gap-4"
			>
				<Icon
					:name="link.icon"
					class="size-8"
				/>
			</NuxtLink>
		</div>
	</div>
</template>

<script setup lang="ts">
const links = [
	{
		name: 'GitHub',
		url: 'https://github.com/fkshohag',
		icon: 'mdi:github',
	},
	{
		name: 'Twitter',
		url: 'https://x.com/shohag_fks',
		icon: 'fa6-brands:square-x-twitter',
	},
	{
		name: 'LinkedIn',
		url: 'https://www.linkedin.com/in/fkshohag/',
		icon: 'mdi:linkedin',
	},
	{
		name: 'Email',
		url: 'mailto:shohag.fks@gmail.com',
		icon: 'mdi:email',
	},
];
</script>

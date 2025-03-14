<template>
	<div
		v-motion-fade-visible
		class="space-y-6"
	>
		<NuxtImg
			src="/shohag-pfl.jpg"
			alt="Md Shohag"
			class="size-12 rounded-full border border-gray-300 bg-gray-200 ring-2 ring-gray-200 transition-all duration-300 hover:ring-4 dark:border-gray-800 dark:bg-gray-900 dark:ring-white/10 sm:size-24"
			placeholder
			width="45"
			format="webp"
			loading="lazy"
		/>
		<h1 class="text-xl font-bold text-gray-800 drop-shadow-2xl dark:text-gray-100">
			Hey. I'm {{ appConfig.name }}. 👋
		</h1> 
		<p class="text-gray-900 dark:text-gray-400">
			I'm a Senior Software Engineer from Bangladesh, with an MSc in Computer Science from 
			<b class="text-primary-700 dark:text-primary-100">Jahangirnagar University</b> 
			and a BSc in Computer Science & Engineering from 
			<b class="text-primary-700 dark:text-primary-100">Southeast University</b>. 
			I specialize in building scalable applications with a strong foundation in DevOps practices and distributed systems.
			<br><br>
			With over 6 years of experience in software design and development, my academic background in algorithms, 
			distributed computing, and AI/ML complements my practical expertise in building high-performance systems. 
			Currently, I'm working with the bKash Engineering team, where we handle Bangladesh's largest Mobile-Financial-Service 
			platform, processing over 18 million daily transactions for 74M+ registered subscribers.
			<br><br>
			My technical expertise spans across multiple domains:
			<br>
			<b class="text-primary-700 dark:text-primary-100">
				Backend: Python, Go, Node.js, PHP,
				<br>
				Frontend: React.js, Vue.js, Angular
				<br>
				DevOps: AWS, GCP, Kubernetes, Docker, Jenkins
				<br>
				Databases: PostgreSQL, MySQL, MongoDB, ScyllaDB
			</b>
			<br><br>
			I have extensive experience architecting microservices, implementing XMPP protocols, and managing cloud infrastructure. 
			I've designed and implemented CI/CD pipelines using Jenkins and worked extensively with both AWS and Google Cloud 
			platforms for deploying highly available applications.
			<br><br>
			Beyond system architecture, I have a strong foundation in algorithmic problem-solving and competitive programming. 
			I've solved 500+ problems across various online judges, which has sharpened my analytical thinking and ability 
			to optimize complex systems.
			<br><br>
			Currently, I'm focused on:
			<br>
			<b class="text-primary-700 dark:text-primary-100">
				• Architecting scalable fintech solutions
				<br>
				• LLM and AI integration in financial services
				<br>
				• High-performance distributed systems
				<br>
				• Algorithmic optimization for large-scale applications
			</b>
			<br><br>
			When I'm not engineering solutions, I enjoy participating in coding competitions, exploring emerging technologies, 
			and contributing to the developer community. I believe in continuous learning and sharing knowledge with others 
			through mentorship and technical discussions.
			<br><br>
			Let's connect! Whether it's about system architecture, algorithmic challenges, or innovative tech solutions, 
			feel free to reach out on <AppExternalLink
				href="https://x.com/shohag_fks"
				title="X account of Md Shohag"
			>
				Twitter
			</AppExternalLink>,
			<AppExternalLink
				href="mailto:shohag.fks@gmail.com"
				title="Email Address Of Md Shohag"
			>
				Email
			</AppExternalLink>!
		</p>
	</div>
</template>

<script setup lang="ts">
import { useSeoMeta } from '#imports';
import appConfig from '~/app.config';

useSeoMeta({
	title: 'Md Shohag',
	description:
		'Senior Software Engineer specializing in scalable applications, system architecture, and DevOps practices with expertise in Python, PHP, and cloud technologies.',
});
</script>

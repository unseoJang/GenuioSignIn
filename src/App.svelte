<script>
	import TailwindCSS from './TailwindCss.svelte'
	import Fa from 'svelte-fa'
	import { faUser,faLock,faEyeSlash } from '@fortawesome/free-solid-svg-icons'
</script>
<TailwindCSS />

<main class="min-h-screen flex items-center justify-center">
	<div class="max-w-screen-sm w-full space-y-12">
		<header class="flex justify-center items-center">
			<img class="transform scale-50 h-auto w-28" src="img/genuio.png" alt="logo">
			<h2 class="font-bold text-6xl">Genuio</h2>
		</header>
		<p>Genuio Design is the most influential web design specification in unseo district</p>
		<form class="mt-4 space-y-8" action="#" method="POST">
			<div class="relative mb-4">
				<label class="max-w-full">
					<input type="text" placeholder="Username:admin or user" class="w-full py-5 pl-10 border-blue-400" />
					<Fa icon={faUser} class="absolute left-4 top-7 text-blue-400 text-xl"/>
				</label>
			</div>
			<div class="relative mb-4">
				<label class="max-w-full">
					<input type="password" placeholder="Password:ant.design" class="w-full py-5 pl-10 border-blue-400"/>
					<Fa icon={faLock} class="absolute left-4 top-6 text-blue-400"/>
					<Fa icon={faEyeSlash} class="absolute right-4 top-6 text-grey-400 text-xl"/>
				</label>
			</div>
			<div class="flex items-center justify-between  ">
				<div class="flex items-center">
					<input type="checkbox" id="rememberMe" class="w-5 h-5 mr-3"/>
					<label for="rememberMe" class="text-xl">Rememeber me</label>
				</div>
				<div class="flex items-center">
					<a href="#" class="text-blue-400">Forgot Password ?</a>
				</div>
			</div>
			<div>
				<button class="w-full flex justify-center py-4 px-4 border-transparent text-sm font-medium rounded-sm text-white bg-blue-500 hover:bg-blue-600" type="submit">Submite</button>
			</div>
		</form>
	</div>
</main>
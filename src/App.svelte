<script lang="ts">
	import Link from './components/Link.svelte'
	let links = [{
		id:"1",
		text:'Google',
		link: 'https://google.com'
	},{
		id:"2",
		text:'Yahoo',
		link: 'https://yahoo.com'
	},{
		id:"3",
		text:'Huvile',
		link: 'https://huvile.com'
	}]
</script>

<main>
	<h1>Super Css Effects</h1>
	<div class="links">
		{#each links as link (link.id)}
		<Link text={link.text} link={link.link}/>
		{/each}
	</div>
</main>

<style>
	
	main {
		padding: 29px;
		background: linear-gradient(109.31deg, #FF7455 0%, #F38A29 100%);
		border-radius: 25px;
	}

	h1 {
		margin:0px;
		font-family: Merriweather;
		font-size: 30px;
		font-style: normal;
		font-weight: 900;
		line-height: 33px;
		letter-spacing: 0em;
		color: #FFFFFF;
		letter-spacing: 2px;
	}

	.links {
		display: flex;
    flex-direction: column;
    margin-top: 1rem;
    grid-gap: 1rem;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
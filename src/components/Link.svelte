<script lang="ts">
  export let text
  export let link
</script>

<a href={link} target="_blank">{text}</a>

<style>
	a {
		font-family: IBM Plex Sans;
font-size: 20px;
font-style: normal;
font-weight: 500;
line-height: 26px;
letter-spacing: 0em;
text-align: left;
color: white;
text-decoration: none;
background: #242640;
border-radius: 10px;
padding: 0.5rem 1rem;
text-align: center;
	}

	a:hover{
			background: #FFDDB6;
			color:#242640;
	}
</style>
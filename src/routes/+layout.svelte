<script>
  import Header from "./Header.svelte";
  import Footer from "./Footer.svelte";
  import './styles.css';
	import Episodes from "./Episodes.svelte";

  export let data;
  $: ({all_episodes} = data)
</script>

<Header />

<main>
  <slot />
  <Episodes episodes={all_episodes} />
</main>

<Footer />
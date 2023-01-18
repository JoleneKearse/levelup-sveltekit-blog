<script>
  import Header from "./Header.svelte";
  import Footer from "./Footer.svelte";
  import './styles.css';

  export let data;
  $: ({all_episodes} = data)
</script>

<Header />

<main>
  <slot />
</main>

<Footer />
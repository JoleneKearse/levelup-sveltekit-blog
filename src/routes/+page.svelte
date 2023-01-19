<script>
  import Test from '$lib/Test.svelte';
  import '$db/start';
  export let data;
  
  $: ({ latest_episode, all_episodes } = data)
</script>

<h3>{latest_episode.title}</h3>

<a href="/about">About Us</a>

<Test />

<style>
  h3 {
    line-height: 1.25;
  }
</style>
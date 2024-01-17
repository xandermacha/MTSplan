<!-- IDK this will be the dash board or sum 
npm install svelte-spa-router 
npm install --save-dev @tauri-apps/cli
npm install --save-dev @sveltejs/adapter-static -->
<script lang="ts">
  import Router from "svelte-spa-router";
  import { push, replace, location } from "svelte-spa-router";
  

  import Home from "./routes/Home.svelte";
  import NewSchedule from "./routes/NewSchedule.svelte";

  let routes = {
    "/": Home,
    "/NewSchedule": NewSchedule,
  }
  const go_home = () => push("/");
  const go_new_schedule = () => push("/NewSchedule");

</script>

<nav>
  <button on:click={go_home}>Home</button>
  <button on:click={go_new_schedule}>New Schedule</button>
</nav>

<main class="container">
  
  <Router {routes} />

</main>

<!-- <style>
  .logo.vite:hover {
    filter: drop-shadow(0 0 2em #747bff);
  }

  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00);
  }
</style> -->
<script lang="ts">
    import Greet from '../lib/Greet.svelte' // switched to reletive path 
</script>
<main class="container">
    <h1>MTSplan</h1>
  
    <div class="row">
      <a href="/">
        <img src="/MTS.png" class="logo mts" alt="MTS Logo" />
      </a>
      <!-- <a href="https://tauri.app" target="_blank"
        <img src="/tauri.svg" class="logo tauri" alt="Tauri Logo" />
      </a>
      <a href="https://svelte.dev" target="_blank">
        <img src="/svelte.svg" class="logo svelte" alt="Svelte Logo" />
      </a> -->
    </div>
  
    <p>
      Click on the Tauri, Vite, and Svelte logos to learn more.
    </p>
  
    <div class="row">
      <Greet />
    </div>
</main>
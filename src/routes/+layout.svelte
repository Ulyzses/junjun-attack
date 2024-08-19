<script lang="ts">
  import '$lib/css/global.css';
</script>

<div class="main-container">
  <slot />
</div>

<style>
  .main-container {
    height: 100vh;
    width: 100vw;

    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    background-color: var(--CURSOR-white);
  }
</style>
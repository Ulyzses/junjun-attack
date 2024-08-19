<script lang="ts">
  export let img: string;
</script>

<div class="chat-container">
  <div class="img-container">
    <img src={img} alt="Player">
  </div>
  <div class="chat-bubble">
    <slot />
  </div>
</div>

<style>
  .chat-container {
    display: flex;
    flex-direction: row;
    margin: 24px;
  }

  .img-container {
    width: 48px;
    height: 48px;

    margin-right: 8px;

    border-radius: 50%;
    border: 2px solid var(--CURSOR-green);
  }

  .img-container img {
    max-height: 100%;
    max-width: 100%;
  }

  .chat-bubble {
    padding: 24px;
    width: 50vw;

    border-radius: 16px;
    border-top-left-radius: 0;

    background-color: #ddd;
  }
</style>
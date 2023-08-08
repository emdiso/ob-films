<script lang="ts">
  import imgSrc from "$lib/assets/image.png";
</script>

<div class="h-screen">
  <div class="flex flex-col h-full justify-center items-center">
    <img style="--height:{35}rem" src={imgSrc} alt="Can't load right now..." />
    <div class="flex justify-center p-1">
      <p class="hover:cursor-text font-bold text-[10px]">
        contact@outerbridgefilms.com
      </p>
    </div>
  </div>
</div>

<style lang="postcss">
  img {
    height: var(--height);
  }
  p {
    font-family: Helvetica;
  }
</style>

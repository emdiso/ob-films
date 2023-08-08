<script lang="ts">
  import imgSrc from "$lib/assets/image.png";
  let heightRem: number = 0;
  let innerWidth = 0;

  $: {
    if (innerWidth <= 480) {
      heightRem = 15;
    } else {
      heightRem = 35;
    }
  }
</script>

<svelte:window bind:innerWidth />

<div class="h-screen">
  <div class="flex flex-col h-full justify-center items-center">
    <img
      style="--height:{heightRem}rem"
      src={imgSrc}
      alt="Can't load right now..."
    />
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

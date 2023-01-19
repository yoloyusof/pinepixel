<script lang="ts">
  import { onMount } from "svelte";

  let selectedColor = "rgb(255,255,255)"

  onMount(() => {
    let elements = document.getElementsByClassName("block");

    for (var i = 0; i < elements.length; i++) {
      let element = elements[i] as HTMLDivElement;

      element.onclick = () => {
        element.style.backgroundColor = selectedColor;
      };
    }
  });
</script>

<main>
  <b-x id="colors">
    <div id="pallete">
      <div class="colorBlock"></div>
    </div>
  </b-x>
  <div id="container">
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
    <div class="block" />
  </div>
</main>

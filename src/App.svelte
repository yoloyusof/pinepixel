<script lang="ts">
  import { onMount } from "svelte";

  let selectedColor = "rgb(255,255,255)"

  onMount(() => {
    let elements = document.getElementsByClassName("block");
    let colors = document.getElementsByClassName("pallete")

    for (var i = 0; i < elements.length; i++) {
      let element = elements[i] as HTMLDivElement;

      element.onclick = () => {
        element.style.backgroundColor = selectedColor;
      };
    }

    for (var i = 0; i < colors.length; i++) {
      let color = colors[i] as HTMLDivElement;

      color.onclick = () => {
        selectedColor = color.style.backgroundColor;
      };
    }
  });
</script>

<main>
  <b-x id="colors">
    <div class="pallete">
      <div class="colorBlock" style="background-color: red;"></div>
      <div class="colorBlock" style="background-color: gray;"></div>
      <div class="colorBlock" style="background-color: white;"></div>
      <div class="colorBlock" style="background-color: green;"></div>
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

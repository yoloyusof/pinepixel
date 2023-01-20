<script lang="ts">
  import { onMount } from "svelte";

  let selectedColor = "rgb(255,255,255)";

  onMount(() => {
    let elements = document.getElementsByClassName("block");
    let colors = document.getElementsByClassName("colorBlock");
    // Determine if mouse is down
    let mouseDown = 0;

    document.onmousedown = function () {
      ++mouseDown;
    };
    document.onmouseup = function () {
      --mouseDown;
    };
    //

    for (var i = 0; i < elements.length; i++) {
      let element = elements[i] as HTMLDivElement;

      element.onmouseover = () => {
        if (mouseDown !== 1) return;
        element.style.backgroundColor = selectedColor;
      };

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

    document.getElementById("tools.clear").onclick = () => {
      for (var i = 0; i < elements.length; i++) {
        let element = elements[i] as HTMLDivElement;

        element.style.backgroundColor = "black"
      }
    }
  });
</script>

<main>
  <b-x id="title">
    <h1>pinepixel</h1>
    <h2>a yusof project</h2>
  </b-x>
  <b-x id="colors">
    <div id="pallete">
      <div class="colorBlock" style="background-color: red;" />
      <div class="colorBlock" style="background-color: gray;" />
      <div class="colorBlock" style="background-color: white;" />
      <div class="colorBlock" style="background-color: green;" />
      <div class="colorBlock" style="background-color: yellow;" />
      <div class="colorBlock" style="background-color: purple;" />
      <div class="colorBlock" style="background-color: orange;" />
      <div class="colorBlock" style="background-color: black;" />
      <div class="colorBlock" style="background-color: brown;" />
      <div class="colorBlock" style="background-color: blue;" />
      <br />
      <div class="colorBlock" id="selectedColorBlock" style="background-color: {selectedColor};" />
    </div>
  </b-x>
  <b-x id="tools">
    <h3>Tools</h3>
    <button id="tools.clear">Clear</button>
  </b-x>
  <div id="container">
    {#each Array(225) as _, i}
      <div class="block" style="background-color: black;" />
    {/each}
  </div>
</main>

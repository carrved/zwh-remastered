<script>
	import "fluent-svelte/theme.css";
	import Buttons from '../lib/Buttons.svelte';
	import { TextBlock } from "fluent-svelte";
	import { onMount } from 'svelte';
	import { fade, scale } from 'svelte/transition';
  
	let ready = false;
	onMount(() => ready = true);
  </script>
  
  <main>
	{#if ready}
	<div>
	  
	</div>
	  <div class="content">
		<center><TextBlock ref="title" variant="display">z4xi's web</TextBlock></center>
	  </div>
	  <center><TextBlock variant="subtitle">biggest gamer website out there :sunglasses:</TextBlock></center>
  
	<div class="buttons">
	  <p in:scale> </p>
	  <center><hr in:scale /></center>
	  <p in:scale> </p>
	  <center><Buttons /></center>
	</div>
	{/if}
  </main>
  
  <style>
	:global([ref=title]) {
	  font-family: monospace;
	}
  </style>
  
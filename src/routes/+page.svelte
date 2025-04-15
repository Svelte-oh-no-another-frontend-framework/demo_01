<script lang="ts">

    let name = $state('world')

    let location = $state('Notch')

	let currentCount = $state(0);
	function add() {
		currentCount++;
	}
</script>

<h1>Welcome to first Notch conference</h1>
<h1>Svelte demo 01</h1>
<br/>
<h2>Osnovni binding</h2>
<p>Hello {name}</p>
<br/>
<h2>Reactive binding</h2>
<input type="text" bind:value={location}>
<p>Hello {name} from {location}</p>
<br/>
<h2>Poziv funkcije</h2>
<p>Clicked {currentCount} times</p>
<button onclick={add}>Dodaj</button>
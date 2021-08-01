<script lang="ts">
	// With the Tauri API npm package:
	import { invoke } from '@tauri-apps/api/tauri';

	// Invoke the command
	invoke('my_custom_command', { invokeMessage: 'Hello!' })
		.then((message) => console.log(message));
	let name: string = 'Fabien';
</script>

<style>
	.name {
		text-transform: capitalize;
	}
</style>

<h1 class="name">Hello {name.toLowerCase()}!</h1>

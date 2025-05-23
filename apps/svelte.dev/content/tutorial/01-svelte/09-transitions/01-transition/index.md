---
title: The transition directive
---

We can make more appealing user interfaces by gracefully transitioning elements into and out of the DOM. Svelte makes this very easy with the `transition` directive.

First, import the `fade` function from `svelte/transition`...

```svelte
/// file: App.svelte
<script>
	+++import { fade } from 'svelte/transition';+++

	let visible = $state(true);
</script>
```

...then add it to the `<p>` element:

```svelte
/// file: App.svelte
<p +++transition:fade+++>
	Fades in and out
</p>
```

---
NOTE: do not edit this file, it is generated in apps/svelte.dev/scripts/sync-docs/index.ts
title: svelte/reactivity/window
---

This module exports reactive versions of various `window` values, each of which has a reactive `current` property that you can reference in reactive contexts (templates, [deriveds]($derived) and [effects]($effect)) without using [`<svelte:window>`](svelte-window) bindings or manually creating your own event listeners.

```svelte
<script>
	import { innerWidth, innerHeight } from 'svelte/reactivity/window';
</script>

<p>{innerWidth.current}x{innerHeight.current}</p>
```



```js
// @noErrors
import {
	devicePixelRatio,
	innerHeight,
	innerWidth,
	online,
	outerHeight,
	outerWidth,
	screenLeft,
	screenTop,
	scrollX,
	scrollY
} from 'svelte/reactivity/window';
```

## devicePixelRatio

<blockquote class="since note">

Available since 5.11.0

</blockquote>

`devicePixelRatio.current` is a reactive view of `window.devicePixelRatio`. On the server it is `undefined`.
Note that behaviour differs between browsers — on Chrome it will respond to the current zoom level,
on Firefox and Safari it won't.

<div class="ts-block">

```dts
const devicePixelRatio: {
	get current(): number | undefined;
};
```

</div>



## innerHeight

<blockquote class="since note">

Available since 5.11.0

</blockquote>

`innerHeight.current` is a reactive view of `window.innerHeight`. On the server it is `undefined`.

<div class="ts-block">

```dts
const innerHeight: ReactiveValue<number | undefined>;
```

</div>



## innerWidth

<blockquote class="since note">

Available since 5.11.0

</blockquote>

`innerWidth.current` is a reactive view of `window.innerWidth`. On the server it is `undefined`.

<div class="ts-block">

```dts
const innerWidth: ReactiveValue<number | undefined>;
```

</div>



## online

<blockquote class="since note">

Available since 5.11.0

</blockquote>

`online.current` is a reactive view of `navigator.onLine`. On the server it is `undefined`.

<div class="ts-block">

```dts
const online: ReactiveValue<boolean | undefined>;
```

</div>



## outerHeight

<blockquote class="since note">

Available since 5.11.0

</blockquote>

`outerHeight.current` is a reactive view of `window.outerHeight`. On the server it is `undefined`.

<div class="ts-block">

```dts
const outerHeight: ReactiveValue<number | undefined>;
```

</div>



## outerWidth

<blockquote class="since note">

Available since 5.11.0

</blockquote>

`outerWidth.current` is a reactive view of `window.outerWidth`. On the server it is `undefined`.

<div class="ts-block">

```dts
const outerWidth: ReactiveValue<number | undefined>;
```

</div>



## screenLeft

<blockquote class="since note">

Available since 5.11.0

</blockquote>

`screenLeft.current` is a reactive view of `window.screenLeft`. It is updated inside a `requestAnimationFrame` callback. On the server it is `undefined`.

<div class="ts-block">

```dts
const screenLeft: ReactiveValue<number | undefined>;
```

</div>



## screenTop

<blockquote class="since note">

Available since 5.11.0

</blockquote>

`screenTop.current` is a reactive view of `window.screenTop`. It is updated inside a `requestAnimationFrame` callback. On the server it is `undefined`.

<div class="ts-block">

```dts
const screenTop: ReactiveValue<number | undefined>;
```

</div>



## scrollX

<blockquote class="since note">

Available since 5.11.0

</blockquote>

`scrollX.current` is a reactive view of `window.scrollX`. On the server it is `undefined`.

<div class="ts-block">

```dts
const scrollX: ReactiveValue<number | undefined>;
```

</div>



## scrollY

<blockquote class="since note">

Available since 5.11.0

</blockquote>

`scrollY.current` is a reactive view of `window.scrollY`. On the server it is `undefined`.

<div class="ts-block">

```dts
const scrollY: ReactiveValue<number | undefined>;
```

</div>




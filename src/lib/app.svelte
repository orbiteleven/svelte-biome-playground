<script lang="ts">
// Biome.js wants to force these to be `import type` because it can't see the Svelte markup
import { FooBar } from "$lib";
import ComponentA from "./component-a.svelte";

// This is why: using these as a type in the `<script>` block causes Biome.js to think they're only being used as type
let fooBar: FooBar;
let component: ComponentA;

// This is a workaround to make Biome.js see that these are being used as values, but is an ugly hack I'd rather NOT use
// const _fooBarImp = FooBar;
// const _componentImp = ComponentA;
</script>

<ComponentA fooBar={FooBar.FOO} />
<script lang="ts">
import { FooBar } from "$lib";
import ComponentA from "./component-a.svelte";

let fooBar: FooBar;
let component: ComponentA;
</script>

<ComponentA fooBar={FooBar.FOO} />
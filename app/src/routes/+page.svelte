<script lang="ts">
let name = 'Svelte';
let count = $state(0);
function handleClick(){
    if (count > 10) {
        alert("You have reached the maximum number of clicks!");
        return;
    }
    count += 1;
}
</script>

<h1> Hello {name}! </h1>
<button onclick={handleClick}>Click me</button>
<p>You clicked the button {count} times.</p>
<script>
    export let clickCount;
    import { createEventDispatcher } from "svelte";
    const dispatch = createEventDispatcher();
    
    function handleClick() {
        dispatch('clickIncrement');
    }
</script>

<button class="test-click-button" on:click={handleClick}>
    Тапай! {clickCount}
</button>

<style>
    .test-click-button {
        background-color: red !important;
        padding: 400px !important;
        color: white !important;
        border: none !important;
        cursor: pointer !important;
    }
</style>
<script>
    function handleClick() {
        alert('Кнопка нажата!');
    }
</script>

<button class="test-button" on:click={handleClick}>
    Нажми меня!
</button>

<style>
    .test-button {
        background-color: blue;
        color: white;
        padding: 20px;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        font-size: 16px;
    }
</style>
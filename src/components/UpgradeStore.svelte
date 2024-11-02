<script>
    export let clickCount;

    const autoClickerCost = 50;
    const clickUpgradeCost = 25;

    function buyClickUpgrade() {
        if (clickCount >= clickUpgradeCost) {
            // улучшение кол-ва тапов за клик
        }
    }
    function buyAutoClicker() {
        if (clickCount >= autoClickerCost) {
            // улучшение автокликера
        }
    }
</script>

<div class="upgrade-menu-container">
    <button class="upgrade-button" on:click={buyClickUpgrade}>Улучшить тап (за {clickUpgradeCost} тапов)</button>
    <button class="upgrade-button" on:click={buyAutoClicker}>Улучшить авто-тап (за {autoClickerCost} тапов)</button>
</div>

<style>
    .upgrade-menu-container {
        display: flex;
        justify-content: center;
        margin-top: 20px;
    }
    
    .upgrade-button {
        margin:  5px;
        padding: 10px 15px;
        border-radius: 5px;
        background-color: #3498db;
        color: white;
        border: none;
        cursor: pointer;
    }

    .upgrade-button:hover {
        background-color: #aa3e1d;
    }
</style>
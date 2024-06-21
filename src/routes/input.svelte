<script>
    import {rawStringToArray} from "./inputLogic";
    let rawInput = '';
</script>

<div class="input-container">
    <form on:submit={rawStringToArray(rawInput)}>
        <label for="sentence-input">Write Something!</label>
        <br><br>
        <input id="sentence-input" type="text" placeholder="Something!" bind:value={rawInput}>
        <br><br>
        <input type="submit" value="Let's get Giffy">
    </form>
</div>

<style>
 .input-container {
        font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        position:absolute;
        top:50%;
        left:50%;
        transform: translate(-50%,-50%);
        padding: 10px;
        border:2px solid white;
        color:white;
    }
</style>
<script>
    let rawInput = '';
    let rawInputTemp = '';
    function handleSubmit() {
        rawInput = rawInputTemp;
        rawInputTemp = '';
    }
</script>

<div class="input-container">
    <form on:submit={handleSubmit}>
        <label for="sentence-input">Write Something!</label>
        <br><br>
        <input type="text" name="sentence-input" placeholder="Something!" bind:value={rawInputTemp}>
        <br><br>
        <input type="submit" value="Let's get Giffy">
    </form>
    <p>{rawInput}</p>
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
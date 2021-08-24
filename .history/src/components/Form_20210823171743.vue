<template>
    <form>
        <input type="text" placeholder="Description...">
        <input type="number" placeholder="Value...">
        <input type="date" placeholder="Date...">
        <input type="submit" value="SUBMIT">
    </form>
</template>

<script>
export default {

}
</script>

<style scoped>
form{
    display: flex;
    justify-content: center;
    margin-top: 30px;
}
form input {
    color: #888;
    border: none;
    outline: none;
    font-size: 20px;
}
form input {
    color: #888;
    border: none;
    outline: none;
    font-size: 20px;
}
form input:placeholder {
    color: #AAA;
}
</style>

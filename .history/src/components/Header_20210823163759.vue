<template>
  <header>
      <h1>Income Tracker</h1>
      <div class="total-income">VND0</div>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped>
header{
    display: flex;
    justify-content:space-between;
    align-items:center;
    padding: 15px 30px;
    background-color: #313131;
    border-bottom: 5px solid #FFCE00;
}
header h1{
    color: #EEE;
    font-size: 28px;
}
header .total-income{
    font-family: 'Fira Code', 'Fira Sans', sans-serif;
    background-color: #FFCE00;
}
</style>

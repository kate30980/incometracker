<template>
  <header>
      <h1>Income Tracker</h1>
      <div class="total-income">${{ totalIncome }}</div>
  </header>
</template>

<script>
export default {
  props: {
      totalIncome:Number,
  }
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
    color: #FFF;
    font-size: 20px;
    font-weight: 900;
    padding: 5px 10px;
    min-width: 100px;
    text-align: center;
    border-radius: 8px;
    box-shadow: inset 0px 0px 6px rgba(0,0,0,0.25);
    text-shadow: 0px 3px 3px rgba(0,0,0,0.25);
}
</style>




<template>
    <div class="income-item">
        <div class="removeItem">x</div>
        <div class="desc">Description...</div>
        <div class="price">$0</div>
        <div class="date">DATE...</div>
    </div>
</template>

<script>
export default {
    props:{
        income: Object,
    }
}
</script>

<style scoped>
.income-item {
    position: relative;
    display: flex;
    padding: 15px 15px 15px 0px;
    background-color:#FFF;
    border-radius: 8px;
    max-width: 600px;
    margin: 0 auto 30px;
}
.removeItem {
    color: #EF2D2D;
    font-weight: 600;
    font-size: 20px;
    line-height: 1.5;
    text-align: center;
    margin: 0 15px;
}
.desc{
    color: #666;
    flex: 1 1 100%;
    font-size: 20px;
}
.price{
    color: #666;
    min-width: 100px;
    font-size: 20px;
}
.date{
    color: #666;
    text-align: right;
    font-size: 20px;
}
</style>







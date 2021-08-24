<template>
  <Header :totalIncome = "state.totalIncome" />
  <Form @add-income = "AddIncome"/>
</template>

<script>
import { reactive, computed } from 'vue';
import Header from './components/Header.vue'
import Form from './components/Form.vue'

export default {
  setup(){
    const state = reactive({
      income: [],
      totalIncome: computed(() => {
        let temp = 0;

        if (state.income.length > 0) {
          for (let i = 0; i < state.income.length; i++) {
            temp += state.income[i].value;
          }
        }

        return temp;
      })
    });

    function AddIncome(data){
      state.income = [...state.income, {
        id: Date.now(),
        desc: data.desc,
        value: data.value,
        date: data.date,
      }]
    }
    
    return{ 
      state
    }
  },
  components: {
    Header, Form
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fira Sans', sans-serif;
}
body{
  background-color: #eee;
}
</style>

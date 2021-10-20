<script>
import store from './store/index.js'
const incr = ()=>{
    store.commit('INCREMENT');
};
const deincr = ()=>{
    store.commit('DEINCREMENT');
};
</script>
<template>
    <div>
        <h2>当前值：{{store.state.count}}</h2>
        <button @click="incr">增加</button>
</template>


<template>
  <div>
    hello info component
    <button type="button" @click="add()">添加</button>
  </div>
</template>

<script>
import store from '@/store';

export default {
  name: 'Info',
  store,
  data() {
    return {
    };
  },
  methods: {
    add() {
      console.log('info button event.');
      store.commit('increase');
    },
  },
};
</script>

<style>
</style>

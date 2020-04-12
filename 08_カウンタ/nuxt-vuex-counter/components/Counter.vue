<template>
  <section>
  <h1>{{title}}</h1>
  Counter:{{ $store.state.counter.counter }}
  <button v-on:click="$store.commit('counter/countUp')">+1</button>
  <button v-on:click="$store.commit('counter/countDown')">リセット</button>
  </section>
</template>

<script>
export default {
  data: function(){
    return {
      title: "Counter App"
    }
  }
}
</script>>
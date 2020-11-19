<template>
  <div id="app">
  </div>
</template>

<script>
export default {
  async created(){
    await this.$store.dispatch("changeDataAction1");
    console.log(this.$store.state.list.data1);
    await this.$store.dispatch("changeDataAction2");
    console.log(this.$store.state.list.data2);
  },
};
</script>
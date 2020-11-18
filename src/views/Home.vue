<template>
  <div id="app"></div>
</template>

<script>
import axios from "axios";
export default {
  async created() {
    let res1=await axios.get("data1.json");
     console.log(res1);
    let res2=await axios.get("data2.json");
     console.log(res2);
  },
}
</script>
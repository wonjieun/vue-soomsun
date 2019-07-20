<template lang="html">
    <div>
        <countValue :cv="num"/>
        <countController @increment="increment" @decrement="decrement"/>
    </div>
</template>
　
<script>
import countValue from "../components/countValue";
import countController from "../components/countController";
export default {
  components: {
    countValue,
    countController
  },
  data() {
    return {
      num: 0
    };
  },
  methods: {
    increment() {
      this.num++;
    },
    decrement() {
      this.num--;
    }
  }
};
</script>
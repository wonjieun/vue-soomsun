<template lang="html">
    <div>
        <button @click="increment">증가</button>
        <button @click="decrement">감소</button>
    </div>
</template>
　
<script>
export default {
  methods: {
    increment() {
      // 부모의 increment라는 이벤트 호출
      this.$emit("increment");
    },
    decrement() {
      // 부모의 decrement 이벤트 호출
      this.$emit("decrement");
    }
  }
};
</script>
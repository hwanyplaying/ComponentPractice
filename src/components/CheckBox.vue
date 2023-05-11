<template>
  <input type="checkbox" :value="value" @click="toggleCheck"/>
</template>

<script>
export default {
  name: "CheckBox",
  props: ['value'],
  methods: {
    toggleCheck() {
      // 1번 emit 사용
      this.$emit('input', !this.value);
      console.log(this.value);
    }
  }
}
</script>

<style scoped>

</style>
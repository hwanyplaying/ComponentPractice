<template>
  <check-box v-model="checked"></check-box>
</template>

<script>


import CheckBox from "@/components/CheckBox.vue";

export default {
  name: 'App',
  components: {
    CheckBox
  },
  data() {
    return {
      checked: false
    }
  },
  /*created() {
    fetchCheckBox()
        .then(function (result) {
          this.checkboxes = result.data;
        })
  }*/
}
</script>

<style>

</style>

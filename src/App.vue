<template>
  <div id="app">
    <div>
      <ul>
        <item>아이템 1</item>
        <item>아이템 2</item>
        <item>아이템 3</item>
        <item>아이템 4</item>
        <item>아이템 5</item>
      </ul>
    </div>
  </div>
</template>

<script>

import Item from "@/Item.vue";

export default {
  name: 'App',
  components: {
    Item
  }
}
</script>

<style>
#app {

}
</style>

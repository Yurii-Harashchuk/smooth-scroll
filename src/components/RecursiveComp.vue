<template>
  <div class="item" v-for="(tree, index) in trees" :key="index">
    <div class="item-title border-bottom">
      {{ tree.title }}
    </div>
    <div v-if="tree.children" class="item-children">
      <RecursiveComp :trees="tree.children"></RecursiveComp>
    </div>
  </div>
</template>

<script setup>
export default {
  name: 'RecursiveComp',
  props: {
    trees: {
      type: Array,
      required: true,
      children: {
        type: Array,
      }
    }
  },
}
</script>

<style>

</style>

<template>
  <div class="viewedit">
    <div contenteditable="true" 
    v-on:input="$emit('input', $event.target.innerHTML)"  v-html="value">{{value}}</div>
  </div>
</template>

<script>
export default {
  name: 'Viewedit',
  props: {
    value: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>

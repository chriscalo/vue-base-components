<!--
  Button.vue
  Author: chris.calo@gmail.com (Chris Calo)
  -->
<template>
  <button type="button" class="Button" v-bind="{ disabled }">
    <slot></slot>
  </button>
</template>

<script>
  export default {
    name: "Button",
    props: {
      disabled: {
        type: Boolean,
        default: false,
      }
    },
  };
</script>

<style scoped>
  .Button[disabled] {
    /* visuals */
    opacity: 0.25;
    
    /* interaction */
    pointer-events: none;
  }
</style>

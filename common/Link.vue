<!--
  Link.vue
  Author: chris.calo@gmail.com (Chris Calo)
  -->
<template>
  <a v-bind="{ href }" class="Link">
    <slot></slot>
  </a>
</template>

<script>
  export default {
    name: "Link",
    props: {
      href: String,
    },
  };
</script>

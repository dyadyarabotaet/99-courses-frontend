<script setup>
defineProps({
  text: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <li class="header-link-wrap">
    <a href="" class="header-link">{{ text }}</a>
  </li>
</template>

<style>
.header-link-wrap {
  margin: auto 0;
}

.header-link {
  font-weight: 700;
  font-size: 15px;
  line-height: 32px;
  color: #f2f7fc;
  text-decoration: none;
}
</style>
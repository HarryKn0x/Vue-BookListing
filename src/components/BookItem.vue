<template>
  <li>{{book.title}}:{{book.author}}</li>
</template>

<style>

</style>

<script>
export default {
  name: 'BookItem',
  props: ['book'],
};
</script>

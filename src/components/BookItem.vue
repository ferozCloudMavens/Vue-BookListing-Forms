<template>
  <li>
    {{book.title}} : {{book.author}} -
    <span v-if="book.finishedReading">Read</span>
    <span v-else>Not Read</span>
    - {{book.ownership}}
  </li>
</template>

<script>
export default {
  name: 'BookItem',
  props: ['book'],
};
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
</style>
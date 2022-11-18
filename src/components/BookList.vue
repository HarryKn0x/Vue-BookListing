<template v-for="book in books">
  <div>
    <h1>{{ title }}</h1>
    <ul>
      <li> {{ books[0].title}}, {{books[0].author }} </li>
      <li> {{ books[1].title}}, {{books[1].author }} </li>
      <li> {{ books[2].title}}, {{books[2].author }} </li>
    </ul>
  </div>
</template>

<style>
h1, h2 {
  font-weight: normal;
}

ul{
  list-style-type: none;
  padding: 0;
}

li{
  display: block;
  margin: 0 10px;
}
</style>

<script>
export default {
  name: 'BookList',
  data() {
    return {
      title: "All Books",
      books: [
        {title: 'Self-Reliance', author: 'Ralph Waldo Emerson'},
        {title: 'American Gods', author: 'Neil Gaiman'},
        {title: 'Amusing Ourselves to Death', author: 'Neil Postman'},
      ]
    };
  },
};
</script>

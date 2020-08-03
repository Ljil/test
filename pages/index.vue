<template>
  <div>
    <h1>Index</h1>
    <article v-for="post in posts" :key="post.id">
      <h2>{{post.title}}</h2>
      <p>{{post.body}}</p>
    </article>
  </div>
</template>

<script>
export default {
  async asyncData({ $axios }) {
    const posts = await $axios.$get(
      "https://jsonplaceholder.typicode.com/posts"
    );
    return { posts };
  },
  data: () => ({
    posts: [],
  }),
  // async mounted() {
  //   this.posts = await this.$axios.$get(
  //     "https://jsonplaceholder.typicode.com/posts"
  //   );
  // },
};
</script>

<style>
article {
  padding: 1rem 3rem;
}
h1 {
  padding: 1rem 1rem 1rem 5rem;
}
</style>

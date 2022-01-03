<template>
  <nuxt-link
    :to="{ name: 'blog-slug', params: {
      sys: id
    }}"
    class="wrapper"
  >
    <article class="card">
      <h1 class="card_title">タイトル</h1>
      <p class="card_text">{{ title }}</p>
      <p class="card_date">{{ date }}</p>
    </article>
  </nuxt-link>
</template>
<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    },
    id: {
      type: String,
      default: ''
    },
    date: {
      type: String,
      default: ''
    }
  }
}
</script>

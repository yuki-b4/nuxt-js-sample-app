<template>
  <section class="index">
    <card 
      v-for="i in 5" 
      :key="i"
    />
  </section>
</template>

<script>
import card from '../components/card.vue'
export default {
  components: { card }
}
</script>

<template>
  <div class="container mx-auto">
    <section class="header">
      <default-header />
    </section>
    <section class="me">
      <me />
    </section>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import DefaultHeader from '~/layouts/Header.vue'
import Me from '~/components/O-MeSection.vue'

export default Vue.extend({
  components: {
    DefaultHeader,
    Me
  }
})
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
</style>

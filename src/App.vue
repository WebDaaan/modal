<template>
  <div class="wrapper">
    <div class="wrapper-content">
      <section>
        <div class="container">
          <!-- first modal -->
          <button class="btn btnPrimary" @click="modalFirst = !modalFirst">Show first modal werbs</button>
          <modals v-if="modalFirst" title="First modal"></modals>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import modals from '@/components/Modal.vue'
export default {
  components: { modals },
  data() {
    return {
      modalFirst: false
    }
  }

}
</script>

<style lang="scss">
/* body {
  background: rgb(204, 226, 233);
  background: linear-gradient(90deg, rgba(204, 226, 233, 1) 0%, rgba(253, 29, 29, 1) 50%, rgba(69, 98, 252, 1) 100%);
} */
</style>
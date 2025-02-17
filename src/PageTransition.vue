<template>
  <div>
    <button @click="testShow = !testShow">
      Show
    </button>
    <div v-if="testShow">
      <button
        @click="testShow = !testShow"
        class="btn-base"
        >
        Hide
      </button>
      <div>
        <div>
          test
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent, ref } from 'vue'

export default defineComponent({
  setup() {
    const testShow = ref(false);

    return { testShow };
  },
})
</script>

<style scoped>
.btn-base {
  transition: opacity 150ms;
}

.btn-base:active {
  opacity: 0.3;
}
</style>

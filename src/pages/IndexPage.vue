<template>
  <q-page class="q-pa-sm">
    <div class="row q-col-gutter-md">
      <div class="col-6">
        <test-component></test-component>
      </div>
      <div class="col-6">
        <test2></test2>
      </div>
    </div>
  </q-page>
</template>

<script>
import {defineComponent, defineAsyncComponent} from 'vue'

export default defineComponent({
  name: 'IndexPage',
  components: {
    TestComponent: defineAsyncComponent(() => import("components/TestComponent.vue")),
    Test2: defineAsyncComponent(() => import("components/Test2.vue"))
  }
})
</script>

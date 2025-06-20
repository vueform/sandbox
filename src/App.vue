<script setup>
import { ref, onMounted } from 'vue'

const form$ = ref()

onMounted(() => {
  console.log(form$.value)
})
</script>

<template>
  <div class="max-w-[500px] mx-auto mt-10">
    <Vueform ref="form$">
      <TextElement name="hello_world" label="Hello" placeholder="World" />
    </Vueform>
  </div>
</template>

<style>
</style>

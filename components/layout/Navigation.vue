<template>
  <nav>
    <ul class="flex">
      <li v-for="(value, key) in $t('navigation')" :key="key" class="mx-6">
        <n-link
          :to="`/${key === 'projects' ? '' : key}`"
          class="font-light uppercase"
        >
          {{ value }}
        </n-link>
      </li>
    </ul>
  </nav>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'Navigation',
})
</script>

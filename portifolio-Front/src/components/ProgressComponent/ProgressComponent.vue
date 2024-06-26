<script setup lang="ts">
import './Progress.scss'
import { defineProps } from 'vue'
import type { ProgressProps } from './Progress.type'

defineProps<ProgressProps>()
</script>
<template>
  <div>
    <p class="textTechnologie">{{ titleProgress }}</p>
    <div class="barraFullProgress" :fullProgress="100">
      <div class="barraProgress" :style="{ width: `${progress}%` }" />
    </div>
  </div>
</template>

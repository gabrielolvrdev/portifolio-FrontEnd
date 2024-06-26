<script setup lang="ts">
import './Card.scss'
import { defineProps } from 'vue'
import type { CardProps } from './Card.type'

defineProps<CardProps>()
</script>

<template>
  <div class="cardProject">
    <div class="imageProject"></div>
    <h6 class="titleProject">
      {{ title }}
    </h6>
    <div class="barraproject"></div>
    <div class="contentTextProject">
      <p class="textProject">
        {{ subtitle }}
      </p>
    </div>
  </div>
</template>

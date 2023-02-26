<script lang="ts" setup>
import { generateRandomExam } from '@/@core/utils'
const randomExam = generateRandomExam()
</script>

<template>
  <p class="text-2xl mb-6">Tao de ngau nhien</p>
  <VCard title="Tao de">
    <VCardText>
      <VForm>
        <!-- Part 1 -->
        <VRow align="center" dense>
          <VCol cols="4">
            <label>Chuong 1 (01-29)</label>
          </VCol>
          <VCol cols="4">
            <VTextField
              :placeholder="`Cau ${randomExam[0]}`"
              :label="`Cau ${randomExam[0]}`"
            />
          </VCol>
          <VCol cols="4">
            <VTextField
              :placeholder="`Cau ${randomExam[1]}`"
              :label="`Cau ${randomExam[1]}`"
            />
          </VCol>
        </VRow>

        <!-- Part 2 -->
        <VRow align="center" dense class="mt-1">
          <VCol cols="4">
            <label>Chuong 2 (30-43)</label>
          </VCol>
          <VCol cols="4">
            <VTextField
              :placeholder="`Cau ${randomExam[2]}`"
              :label="`Cau ${randomExam[2]}`"
            />
          </VCol>
        </VRow>
      </VForm>
    </VCardText>
  </VCard>
</template>

<style lang="scss"></style>

<script setup>
import { ref } from 'vue'

const nome = ref('')
</script>

<template>
  <main class="flex min-h-screen items-center justify-center bg-surface-100 p-6">
    <Card class="w-full max-w-md">
      <template #title>
        Cadastro
      </template>

      <template #content>
        <div class="flex flex-col gap-4">
          <InputText
            v-model="nome"
            placeholder="Digite seu nome"
            fluid
          />

          <Button
            label="Cadastrar"
            icon="pi pi-check"
          />
        </div>
      </template>
    </Card>
  </main>
</template>
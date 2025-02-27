<template>
  <div class="p-4 flex-1 overflow-y-auto">
    <div class="flex flex-col space-y-2">
      <ChatBullula :meus-est="true" nuntius="¿Salimos luego a dar una vuelta?" />
      
      <ChatBullula
        :meus-est="false"
        nuntius="no"
        imago="https://yesno.wtf/assets/yes/5-64c2804cc48057b94fd0b3eaf323d92c.gif"
      />
    </div>
  </div>
</template>

<script lang="ts" setup>
import ChatBullula from './ChatBullula.vue';
</script>

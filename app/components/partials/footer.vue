<template>
  <footer class="footer -mx-4 md:mx-0">
    <div class="container mx-auto pb-6 flex justify-center">
      <nuxt-link to="https://cedille.pro">
        <img :src="cedille" alt="Logo Cédille" />
      </nuxt-link>
    </div>
  </footer>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';
import settings from '@/content/settings/general.json';

@Component
export default class Footer extends Vue {
  cedille = settings.cedille;
}
</script>

<style lang="scss">
.footer {
  background-color: $bluise;
}
</style>

<template>
  <footer
    class="relative p-5 text-center border-t shadow border-clrSecondary md:pd-6"
  >
    <span class="text-sm text-gray-500">
      Alok Ranjan Thakur © {{ currentYear }} | Made with love using VueJS and Tailwind
    </span>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      currentYear: new Date().getFullYear()
    };
  }
};
</script>

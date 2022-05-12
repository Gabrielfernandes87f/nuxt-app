<template>
  <div class="slots-base">
    <header class="header">
      <HeaderComponent />
    </header>

    <main class="main">
      <slot />
    </main>

    <footer class="footer">footer</footer>
  </div>
</template>

<script>
import HeaderComponent from "~/components/HeaderComponent.vue";
export default {
  components: { HeaderComponent },
  name: "DefaultLayout",
};
</script>

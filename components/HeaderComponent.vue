<template>
  <div id="header">
    <div class="nav">
      <ul class="nav-ul">
        <li class="ul-li">
          <nuxt-link to="#" class="li-links">Home</nuxt-link>
        </li>
        <li class="ul-li">
          <nuxt-link to="#" class="li-links">Sobre</nuxt-link>
        </li>
        <li class="ul-li">
          <nuxt-link to="#" class="li-links">Contato</nuxt-link>
        </li>
        <li class="ul-li">
          <nuxt-link to="#" class="li-links">Jobs</nuxt-link>
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  name: "hearderComponent",
  props: {
    title: {
      type: String,
      default: "Bulma Vue",
    },
  },
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isActive = !this.isActive;
      console.log(this.isActive);
      if (this.isActive) {
        document.body.classList.add("toggle-menu");
      } else {
        document.body.classList.remove("is-menu-open");
      }
    },
  },
};
</script>
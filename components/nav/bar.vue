<template>
  <nav>
    <div class="nav">
      <NuxtLink to="/">
        <div class="nav__icon nav__elm">
          <img src="/images/xuyuan_icon.png" class="nav__icon__pic" alt="" />
          <div class="nav__icon__text">
            <span class="nav__icon__name">Tang Xuyuan</span>
            <span class="nav__icon__title">Student | Programmer</span>
          </div>
        </div>
      </NuxtLink>

      <a
        class="nav__menu nav__elm"
        :class="{ 'nav__menu--open': isMenuOpen }"
        @click="menuClick"
      >
        <MenuIcon class="open" size="26" />
        <CloseIcon class="close" size="26" />
      </a>
    </div>
    <div class="menu" :class="{ 'menu--shown': isMenuOpen }">
      <ul class="links">
        <li><NuxtLink to="/" @click="menuClick">Home</NuxtLink></li>
        <li>
          <NuxtLink to="/#experience" @click="menuClick">Experience</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/#tech-skills" @click="menuClick">Tech Skills</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/#academic" @click="menuClick">Academic</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/#contact" @click="menuClick">Contact Me</NuxtLink>
        </li>
      </ul>
    </div>
    <br class="nav-spacer" />
  </nav>
</template>

<script setup>
import MenuIcon from "vue-material-design-icons/Menu.vue";
import CloseIcon from "vue-material-design-icons/Close.vue";
import { ref } from "vue";
const isMenuOpen = ref(false);
function menuClick() {
  isMenuOpen.value = !isMenuOpen.value;
  //TODO: stop page scroll when modal open
}
</script>

<style scoped>
.nav {
  position: fixed;

  z-index: 100;
  margin-bottom: 1rem;
  top: 0;
  left: 0;
  right: 0;
  background-color: rgba(var(--bg-rgb), 0.95);
  box-shadow: 0px 0px 10px 4px rgba(var(--fg-rgb), 0.2);
  overflow: hidden;

  border-bottom: 1px solid var(--fg);
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: clamp(1.5rem, calc(2.5vw - 1rem), 3rem);
  padding-bottom: 0;
}
.nav__elm {
  padding: 1rem;
}
.nav > a::after {
  display: none;
}
.nav__menu {
  width: 30px;
  display: flex;
  z-index: 111;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  --trn: var(--trn-time) top ease-out, var(--trn-time) bottom ease-out,
    var(--trn-time) opacity ease-out;
  --trn-time: 600ms;
}
.nav__menu .open {
  transition: var(--trn);
  position: absolute;
  bottom: calc(50% - 16px);
  opacity: 1;
}
.nav__menu .close {
  transition: var(--trn);
  position: absolute;
  top: 150%;
  opacity: 0;
}
.nav__menu.nav__menu--open .open {
  bottom: 150%;
  opacity: 0;
}
.nav__menu.nav__menu--open .close {
  top: calc(50% - 13px);
  opacity: 1;
}

.nav__icon {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 0.75rem;
}
.nav__icon__pic {
  border-radius: 50%;
  border: 1px solid var(--fg);
  --size: clamp(37px, 4.5vw, 52px);
  width: var(--size);
  height: var(--size);
}
.nav__icon__text {
  display: flex;
  flex-direction: column;
  gap: 0.25rem;
}
.nav__icon__name {
  font-weight: 700;
  font-size: 20px;
}
.nav__icon__title {
  font-size: 9px;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 0.15rem;
}

.menu {
  position: fixed;
  z-index: 99;
  width: 100%;
  height: 100%;
  left: 0;
  top: 100%;
  background-color: rgba(var(--bg-rgb), 0.99);
  --trn-func: cubic-bezier(0.29, 0.11, 0.06, 1);
  --trn-time: 600ms;
  transition: top var(--trn-time) var(--trn-func);
  border-block: 1px solid rgba(var(--fg-rgb), 50%);
  display: flex;
  align-items: center;
  justify-content: center;
}
.menu--shown {
  top: 0;
}
.menu .links {
  list-style: none;
  padding-left: 0;
  text-align: center;
  font-weight: bold;
  font-size: 24px;
  opacity: 0;
  transition: opacity var(--trn-time) var(--trn-func);
}

.menu .links::before {
  display: block;
  margin-bottom: 1rem;
  content: "Menu";
  text-transform: uppercase;
  font-size: 14px;
  font-weight: 300;
  letter-spacing: 0.25rem;
}
.menu--shown .links {
  opacity: 1;
}
.menu .links * {
  margin-bottom: 1.5rem;
  color: rgba(var(--fg-rgb), 0.6);
  transition: 200ms color ease-in-out;
}
.menu .links *:hover {
  color: var(--fg);
}
.menu .links *:hover::after {
  display: none;
}

.nav-spacer {
  margin-block: 2rem;
}

@media screen and (min-width: 800px) {
  .nav {
    position: fixed;
    border: none;
    background-color: transparent;
    box-shadow: none;
  }
  .nav__elm {
    border: 1px solid var(--fg);
    background-color: rgba(var(--bg-rgb), 0.9);
    box-shadow: 0px 0px 10px 4px rgba(var(--fg-rgb), 0.2);
    border-radius: 0.25rem;
  }
  .nav__elm:hover {
    color: var(--fg-secondary);
  }
  .nav__menu {
    --size: 1.25rem;
    width: var(--size);
    height: var(--size);
    --trn-time: 400ms;
  }
  .nav__menu .close {
    top: 100%;
    opacity: 0.4;
  }
  .nav__menu--open .open {
    bottom: 100%;
    opacity: 0.4;
  }

  .nav-spacer {
    margin: 0;
  }

  .menu .links {
    font-size: 32px;
  }
}
</style>

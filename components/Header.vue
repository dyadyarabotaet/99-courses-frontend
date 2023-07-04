<script setup lang="ts">
const links = [
  {
    text: "Home",
  },
  {
    text: "Courses",
  },
  {
    text: "Pricing",
  },
  {
    text: "FAQ",
  },
  {
    text: "About Us",
  }
]
</script>

<template>
  <header class="page-header">
    <nav class="header-navigation">
      <LogoLink />

      <ul class="header-navigation-list">
        <HeaderLink v-for="link in links" :key="link.text" :text="link.text" />
      </ul>

      <div class="header-navigation-button-group">
        <LogInButton />
        <EnrollButton />
      </div>
    </nav>
  </header>
</template>

<style>
.page-header {
  position: sticky;
  width: auto;
  height: 80px;
  padding: 0 80px;
  background: linear-gradient(0deg, var(--color-primary), #0c2445), #0d1c33;
}

.header-navigation {
  display: flex;
  position: relative;
  height: 80px;
}

.header-navigation-list {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  margin: 0;
  padding: 0px;
  gap: 32px;

  position: absolute;
  width: 500px;
  height: 56px;
  left: calc(50% - 500px / 2 - 0px);
  top: calc(50% - 56px / 2);

  list-style: none;
}

.header-navigation-button-group {
  display: flex;
  flex-direction: row;
  align-items: center;
  padding: 0px;
  gap: 32px;

  position: absolute;
  width: 230px;
  height: 64px;
  right: 0px;
  top: calc(50% - 64px / 2);
}
</style>
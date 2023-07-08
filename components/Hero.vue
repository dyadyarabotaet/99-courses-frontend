<script></script>

<template>
  <section class="hero">
    <div class="hero-content">
      <h1 class="hero-heading">Grow your community with 99Rows</h1>
      <p class="hero-discription">
        99Rows is a flexible learning management system (LMS) template with
        everything you need to sell video content. Create an entire catalogue or
        just a single course and sell subscriptions with ease!
      </p>
      <HeroButton />
    </div>
  </section>
</template>

<style>
.hero {
  display: flex;
  position: relative;
  height: 883px;
  padding: 80px;
  flex-direction: column;
  align-items: center;
  gap: 40px;
  align-self: stretch;
  background-image: url("../img/hero_layout.jpg");
}

.hero::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    180deg,
    #0d1c33 11.46%,
    rgba(13, 28, 51, 0.8) 40.1%,
    rgba(13, 28, 51, 0) 100%
  );
}

.hero-content {
  display: flex;
  width: 800px;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 28px;
  z-index: 2;
}

.hero-heading {
  display: flex;
  width: 100%;
  height: auto;
  flex-direction: column;
  margin: 0;
  align-self: stretch;
  text-align: center;
  font-size: 77px;
  font-weight: 700;
  line-height: 120%;
}

.hero-discription {
  display: flex;
  flex-direction: column;
  margin: 28px 0;
  align-self: stretch;
  text-align: center;
  font-size: 22px;
  line-height: 140%;
}
</style>

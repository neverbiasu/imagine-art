<template>
  <div
    class="min-h-[1024px] bg-gradient-to-b from-[#E6F7F5] to-white font-['Microsoft YaHei']"
  >
    <section
      class="pt-36 min-h-[600px] flex items-center relative bg-cover bg-center banner"
    >
      <div class="max-w-[1440px] mx-auto px-8 py-16 relative z-10">
        <div class="max-w-lg">
          <h1 class="text-5xl font-bold text-gray-800 mb-6">AI 智能创作平台</h1>
          <p class="text-xl text-gray-600 mb-8">
            使用先进的 AI
            技术，轻松创作独特的插画作品。无需专业技能，让创意自由绽放。
          </p>
          <NuxtLink
            to="/generate"
            class="inline-flex items-center px-8 py-3 bg-primary text-gray-800 font-medium rounded-xl hover:bg-opacity-90 transition-all shadow-md hover:shadow-lg border-2 border-blue-200"
          >
            开始创作
            <font-awesome-icon :icon="['fas', 'arrow-right']" class="ml-2" />
          </NuxtLink>
        </div>
      </div>
    </section>

    <section class="py-16">
      <div class="max-w-7xl mx-auto px-6">
        <h2 class="text-2xl font-bold text-gray-800 mb-8">精选案例</h2>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
          <div
            class="rounded-lg overflow-hidden shadow-lg transition-all hover:shadow-xl hover:-translate-y-1"
          >
            <img
              src="/images/examples/response1.png"
              alt="案例1"
              class="w-full h-[300px] object-cover"
            />
          </div>
          <div
            class="rounded-lg overflow-hidden shadow-lg transition-all hover:shadow-xl hover:-translate-y-1"
          >
            <img
              src="/images/examples/response2.png"
              alt="案例2"
              class="w-full h-[300px] object-cover"
            />
          </div>
          <div
            class="rounded-lg overflow-hidden shadow-lg transition-all hover:shadow-xl hover:-translate-y-1"
          >
            <img
              src="/images/examples/response3.png"
              alt="案例3"
              class="w-full h-[300px] object-cover"
            />
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
.hero-section {
  background-image: url('/images/hero-bg.jpg');
  background-size: cover;
  background-position: center;
}
.banner::after {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-image:
    linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 0.1)),
    url('/images/teaser.png');
  background-size: cover;
  background-position: center;
}
</style>

<template>
  <div class="container">
    <div class=" flex flex-row w-3/4">
      <transition appear name="delay-appear-profile">
        <img class="profile inline-flex rounded opacity-50" src="~assets/images/ojikun.JPG">
      </transition>

      <transition appear name="delay-appear-contents">
        <div class="flex flex-col ml-10">
          <h2 class="text-4xl">Ojikun's Portfolio yeah I'm Japanese "Paripi"</h2>
          <h4 class="text-orange-700">"Paripiを知らない人は<a href="/">こちら</a>を参照してください。</h4>
          <p class="mt-5">
            4年生を卒業後、新卒でIT系の会社へ就職。約8ヶ月、ITインフラの法人営業を経験。<br>
            入社とほぼ同時にプログラミングを学びはじめ、時間を忘れて夢中になれることから<br>Web系エンジニアへ転身。<br>
            現在はレジャーホテルの開発に携わっております。
          </p>
        </div>
      </transition>
    </div>
    <transition appear name="delay-appear-title">
      <div class="title-section flex flex-col">
        <h1 class="title-section-service">Servicecs</h1>
        <h2 class="title-section-desc">Create and support your web product.</h2>
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  transition: {
    name: 'delay-appear-profile',
    name: 'delay-appear-contents',
    name: 'delay-appear-title'
  },
  mode: 'out-in'
}
</script>

<style scoped>
.profile {
  background-size: cover;
  height: 200px;
  width: 200px;
}

.container {
  margin: 100px 100px 30px 100px;
  padding: 50px 0 0 50px;
}

.title-section {
  position: relative;
}

.title-section-service {
  color: #101010;
  font-size: 180px;
  padding: 120px 50px 0 50px;
}

.title-section-desc {
  font-size: 20px;
  position: absolute;
  top: 295px;
  left: 55px;
}

.delay-appear-profile-enter {
  opacity: 0;
}

.delay-appear-profile-enter-active {
  transition: 10s;
  opacity: 0.5;
}

.delay-appear-contents-enter {
  opacity: 0;
}

.delay-appear-contents-enter-active {
  transition: 6s;
}

.delay-appear-title-enter {
  opacity: 0;
}

.delay-appear-title-enter-active {
  transition: 4s;
}
</style>

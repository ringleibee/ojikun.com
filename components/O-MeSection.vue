<template>
  <div class="container flex flex-row w-3/4">
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
</template>

<script>
export default {
  transition: {
    name: 'delay-appear-profile',
    name: 'delay-appear-contents'
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
  margin: 100px;
  padding: 50px 0 100px 50px;
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
</style>

<template>
  <div class="container mx-auto">
    <div class="flex flex-col w-full items-center">
      <!-- web cording section -->
      <h1 class="title-1 text-5xl mb-5">- Website cording -</h1>
      <p class="title-desc-1 w-2/3">
        HTML、CSS、jQueryを用いてオリジナルのホームページを作成致します。<br>
        SEOを意識したコーディング、迅速な納品を心がけております。Sass等も対応しております。<br>
        お客様でご用意して頂くモノはデザインデータのみです。
      </p>

      <!-- web scraping section -->
      <h1 class="title-2 text-5xl mb-5">- Web scraping -</h1>
      <p class="title-desc-2 w-2/3">
        Pythonを用いたスクレイピング技術利用し、公開されているwebサイトから定期的な情報の取得を致します。<br>
        Amazonで売れているモノをリサーチしたり、WEARで最新のトレンドを掴めたりと、色々な事ができます。<br>
        また、ブラウザの操作自動化も承っています。<br>
        マッチングアプリの足跡自動化、ECサイトの自動カート追加等できます。
      </p>

      <h1 class="title-3 text-5xl mb-5">- Web Application developping -</h1>
      <p class="title-desc-3 w-2/3">
        Vue.jsやLaravelなど、最新の技術を用いてストレスフリーなwebアプリケーションの構築を
        フロントエンドから<br>バックエンドまでサポートさせて頂きます。
        お気軽にまずはご相談ください。
      </p>
    </div>

      <div class="title-section flex flex-row-reverse">
        <h1 class="title-section-skills">Skills</h1>
        <h2 class="title-section-desc">My skills and how much masterd</h2>
      </div>
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
.container {
  margin: 0 100px 30px 100px;
}

.title-2 {
  margin-top: 175px;
}

.title-3 {
  margin-top: 175px;
}

.title-section {
  position: relative;
}

.title-section-skills {
  color: #101010;
  font-size: 180px;
  padding: 120px 50px 0 50px;
}

.title-section-desc {
  font-size: 20px;
  position: absolute;
  top: 295px;
  right: 55px;
}

</style>

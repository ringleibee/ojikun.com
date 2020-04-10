<template>
  <header class="header">
    <nav class="nav">
      <div class="flex flex-col lg:flex-row items-center justify-between">
        <transition appear name="delay-appear-title">
          <nuxt-link
            to="/"
            class="text-primary-500 text-center p-3 pb-1 lg:pb-3 lg:text-left hover:opacity-75"
          >
            <h1 class="text-3xl font-leckerli-one">
              Ojikun.com
            </h1>
            <p class="lg:block text-sm">
              Web developping
            </p>
          </nuxt-link>
        </transition>
        <transition appear name="delay-appear-menulink">
          <div class="block text-primary-500">
            <ul class="flex font-quicksand">
              <li class="menu-link">
                <nuxt-link
                to="/"
                >
                  Me
                </nuxt-link>
              </li>

              <li class="menu-link">
                <nuxt-link
                to="/"
                >
                  Services
                </nuxt-link>
              </li>

              <li class="menu-link">
                <nuxt-link
                to="/"
                >
                  Projects
                </nuxt-link>
              </li>

              <li class="menu-link">
                <nuxt-link
                to="/"
                >
                  Skills
                </nuxt-link>
              </li>

              <li class="menu-link">
                <nuxt-link
                to="/"
                >
                  Contact
                </nuxt-link>
              </li>
            </ul>
          </div>
        </transition>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  transition: {
    name: 'delay-appear-title',
    name: 'delay-appear-menulink'
  },
  mode: 'out-in'
}
</script>

<style scoped>
/* .header {
  @apply w-full z-10;
}
.nav {
  @apply w-full items-center justify-between flex-wrap;
} */
.menu-link {
  @apply relative inline-block no-underline mx-5 text-xl pb-2;
}
.menu-link::after {
  @apply absolute left-0 w-full;
  bottom: -6px;
  content: '';
  height: 4px;
  background: white;
  transform: scale(0, 1);
  transform-origin: left top;
  transition: transform 0.5s;
}
.menu-link:hover::after {
  transform: scale(1, 1);
}

.delay-appear-title-enter {
  opacity: 0;
}

.delay-appear-title-enter-active {
  transition: 2s;
}

.delay-appear-menulink-enter {
  opacity: 0;
}

.delay-appear-menulink-enter-active {
  transition: 4s;
}
</style>

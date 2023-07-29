<template>
  <header class=""></header>
  <main class="mt-24">
    <div class="m-auto max-w-2xl">
      <h1 class="text-6xl font-bold headline">Hey, I'm Jean-Pierre Carvalho</h1>
      <article class="mt-6">
        <div class="text-md">
          <div class="mt-0">
            <p>
              Yo, what's up? Jean-Pierre in the house, proudly rocking the
              developer vibe! 👨‍💻
            </p>
          </div>
          <div class="mt-4">
            <p>What I am? A Staff Frontend Engineer</p>
            <p>Where? In Porto, Portugal 🇵🇹</p>
            <p>
              Working at
              <a href="https://team.emma-sleep.com/about-emma" target="_blank"
                >Emma Sleep Company</a
              >
            </p>
          </div>
          <div class="mt-8">
            <p>
              I'm all about that code life! I'm constantly whipping up fresh
              indie projects just for kicks. My ultimate aim? Easy peasy – to
              craft awesome stuff alongside awesome folks!
            </p>
          </div>
          <div class="mt-8">
            <p>
              When I ain't busy coding, I love kicking back, watching movies,
              and going on adventures! 🚀🎬 If you're chillin' in Porto like me,
              we should totally link up! We can grab some drinks or code
              together, whichever floats your boat. Hit me up! 🍻💻
            </p>
          </div>
        </div>
      </article>
    </div>
  </main>
  <footer class="m-auto max-w-2xl mt-24">
    {{ current_year }} © Jean-Pierre Carvalho
  </footer>
</template>

<script setup lang="ts">
useHead({
  title: 'Intro Page',
  meta: [{ name: 'jeanpierrecarvalho.pt', content: 'My amazing site.' }],
})
const current_year = new Date().getFullYear()
</script>

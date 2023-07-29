<template>
  <header class=""></header>
  <main class="mt-24">
    <div class="m-auto max-w-2xl">
      <h1 class="text-6xl font-bold headline">Hey, I'm Jean-Pierre Carvalho</h1>
      <h2 class="text-4xl font-bold mt-4">
        Staff Frontend Engineer at Emma Sleep
      </h2>
      <article class="mt-6">
        <div class="text-md">
          <div class="mt-0">
            <p>
              Hey there, I'm a super passionate Staff Frontend Developer,
              currently living it up in beautiful Portugal. I've got over 10
              years of experience under my belt, and my main focus has been on
              agile development, top-notch architecture, and building awesome
              teams. I'm all about crafting software products that not only work
              like a charm but also look absolutely stunning! 😎🚀
            </p>
          </div>
          <div class="mt-4">
            <p>
              Before diving headfirst into software stuff, I was all about being
              a mechatronics whiz, dreaming of crafting cool robots. But when I
              finally rolled up my sleeves and began coding those bots, it hit
              me like a bolt of lightning—I was absolutely smitten with software
              development! From that moment on, I was hooked and couldn't stop
              gobbling up everything there was to know about it.
            </p>
          </div>
          <div class="mt-4">
            <p>
              When I'm not knee-deep in code, you'll find me chillin' with my
              girlfriend and my dog in Portugal or jet-setting around the world.
              I'm into binge-watching TV shows and movies, gaming it up with my
              buds, or just hanging out with them. I'm all about being curious
              and digging deep, so I tinker with side projects, contribute to
              open-source software, and always strive to level up my skills. Oh,
              and after a hard day at the office, I love cookin' up some fresh,
              tasty grub at home. Yum! 🍔🍕🍲
            </p>
          </div>
          <div class="mt-4">
            <p>
              I'm all about that code life! I'm constantly whipping up fresh
              indie projects just for kicks. My ultimate aim? Easy peasy – to
              craft awesome stuff alongside awesome folks!
            </p>
          </div>
        </div>
      </article>
      <h2 class="text-4xl font-bold mt-16">
        My Crazy Ride Through the Coding World!
      </h2>
      <div class="mt-8 w-full border-2 p-4" v-for="job in jobs">
        <div class="flex transition-all transform md:hover:scale-[1.01]">
          <div
            class="glass-light drop-shadow-lg hover:drop-shadow-2xl transition-all w-full"
          >
            <div class="flex flex-row items-start md:items-center">
              <div class="flex flex-row mb-2 w-full">
                <div class="flex flex-col w-4/6 justify-between">
                  <h3 class="font-bold">
                    {{ job.role }}
                  </h3>
                  <h4>
                    {{ job.company }}
                    <!-- <a
                      href="https://lexir.com/"
                      target="_blank"
                      rel="noopener noreferrer"
                      class="underlined relative"
                    >
                      </a
                    > -->
                  </h4>
                </div>
                <div class="w-2/6">
                  <span class="text-sm md:text-base">
                    {{ job.timePeriod }}</span
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <h2 class="text-4xl font-bold mt-16">Check Out My Badges</h2>
      <div
        class="mt-8 w-full border-2 p-4"
        v-for="certification in certifications"
      >
        <div class="flex transition-all transform md:hover:scale-[1.01]">
          <div
            class="glass-light drop-shadow-lg hover:drop-shadow-2xl transition-all w-full"
          >
            <div class="flex flex-row items-start md:items-center">
              <div class="flex flex-row mb-2 w-full">
                <div class="flex flex-col w-4/6 justify-between">
                  <h3 class="font-bold">
                    {{ certification.title }}
                  </h3>
                  <h4>
                    {{ certification.company }}
                    <!-- <a
                      href="https://lexir.com/"
                      target="_blank"
                      rel="noopener noreferrer"
                      class="underlined relative"
                    >
                      </a
                    > -->
                  </h4>
                </div>
                <div class="w-2/6">
                  <span class="text-sm md:text-base">
                    {{ certification.timePeriod }}</span
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
  <footer class="m-auto max-w-2xl mt-24">
    {{ current_year }} © Jean-Pierre Carvalho
  </footer>
</template>

<script setup lang="ts">
const current_year = new Date().getFullYear()
const jobs = [
  {
    role: 'Staff Frontend Engineer',
    timePeriod: 'Jan 2023 — Present',
    company: 'Emma Sleep',
  },
  {
    role: 'CTO (Co-founder) & Software Architect',
    timePeriod: 'Aug 2021 — Oct 2022',
    company: 'Lexir',
  },
  {
    role: 'CTO (Founder) & Software Architect',
    timePeriod: 'Aug 2019 — Dec 2022',
    company: 'Plug With Us',
  },
  {
    role: 'CTO & Software Architect',
    timePeriod: 'Sept 2017 — Jan 2020',
    company: 'IHTP',
  },
  {
    role: 'Web Optimization Coordinator & Developer',
    timePeriod: 'Nov 2016 — Sept 2017',
    company: 'Sonae (Bit)',
  },
  {
    role: 'Tech Lead & FullStack Developer',
    timePeriod: 'Jan 2016 — Nov 2016',
    company: 'Actuarial Group',
  },
  {
    role: 'System Administrator & Fullstack Developer',
    timePeriod: 'Jan 2015 — Dec 2015',
    company: 'Lactogal',
  },
  {
    role: 'Freelancer FullStack Developer',
    timePeriod: 'Sept 2011 - Dec 2014',
    company: 'Multiple projects',
  },
  {
    role: 'Telecommunication Expert',
    timePeriod: 'Sept 2010 — Sept 2011',
    company: 'Portuguese Army',
  },
]
const certifications = [
  {
    title: 'User Experience & User Interface Design',
    timePeriod: 'Jan 2019',
    company: 'Edit',
  },
  {
    title: 'Electronic and Computers Enginnering Degree',
    timePeriod: 'Sept 2011 - Jul 2015',
    company: 'Lusiada University',
  },
]
</script>

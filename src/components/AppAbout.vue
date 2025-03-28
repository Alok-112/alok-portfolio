<template>
  <section id="about" class="overflow-hidden text-clrSecondary">
    <div class="mx-auto max-w-7xl">
      <h2
        class="text-3xl font-bold text-center text-clrSecondary md:text-left md:text-4xl"
      >
        About
      </h2>
      <div
        class="flex flex-col-reverse gap-5 text-center md:text-left md:flex-row"
      >
        <div
          data-aos="fade-up"
          data-aos-offset="0"
          data-aos-duration="1000"
          data-aos-easing="ease-in-out"
          data-aos-mirror="true"
          data-aos-once="true"
          class="w-full md:w-1/2"
        >
          <p class="max-w-2xl mx-auto leading-8 text-clrSecondary">
            Hi, I’m Alok. A passionate frontend developer, always eager to
            explore new technologies and push my boundaries. I consider myself a
            fast learner, able to grasp new concepts quickly with an excellent
            ability to retain knowledge.
            <br /><strong
              >My tech stack in short includes: JavaScript, TypeScript, VueJS,
              NextJS, Tailwind, CSS, and Firebase.</strong
            >
          </p>

          <br />
          <button
            v-show="!readMore"
            @click="readMore = !readMore"
            class="text-clrAccent"
          >
            <u> Read More</u>
          </button>
          <Transition name="slide-fade">
            <div v-show="readMore">
              <p class="max-w-2xl mx-auto leading-8 text-clrSecondary">
                My journey into tech started out of pure curiosity. I didn’t
                have a formal degree in computer science, but I was always
                fascinated by how websites and apps worked behind the scenes.
                <br />
                I began with the basics—learning HTML, CSS, and JavaScript from
                free resources online. At first, it was just a hobby, but soon I
                realized this was something I wanted to pursue seriously.
                <br />
                I dived into frontend development, exploring Vue.js and React,
                and then moved to backend with Node.js and databases like
                MongoDB. I worked on small projects, built personal websites,
                and even contributed to open-source to sharpen my skills.
                <br />
                Knowing I had to prove myself through real-world work, I started
                freelancing and building projects to showcase my abilities. The
                more I coded, the more I fell in love with problem-solving and
                web development.
                <br />
                My journey is still ongoing, and every day, I'm learning,
                building, and growing. This is just the beginning, and I’m
                excited to see where this path leads me!
              </p>
              <button @click="readMore = !readMore" class="text-clrAccent">
                <u>Hide it, please</u>
              </button>
            </div>
          </Transition>
        </div>
        <div class="md:w-1/2">
          <div class="w-full px-10 lg:px-20">
            <img
              data-aos="fade-down"
              data-aos-offset="0"
              data-aos-duration="1000"
              data-aos-easing="ease-in-out"
              data-aos-mirror="true"
              data-aos-once="false"
              data-aos-anchor-placement="top-center"
              class="rounded-md md:w-full lazy"
              src="/nikola_profile.jpg"
              alt="Nikola G. Profile Photo"
            />
          </div>
          <p
            class="mt-2 text-sm leading-8 sm:text-center text-clrSecondaryLight"
          >
            "Built through code, driven to create <br />
            Every project, a step toward great"
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';
import '@heroicons/vue/24/outline';

const readMore = ref(false);
</script>

<style>
.slide-fade-enter-active {
  transition: all 0.3s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.8s cubic-bezier(1, 0.5, 0.8, 1);
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(20px);
  opacity: 0;
}
</style>

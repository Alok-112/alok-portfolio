<template>
  <div
    data-aos="fade-right"
    data-aos-offset="0"
    data-aos-duration="1000"
    data-aos-easing="ease-in-out"
    data-aos-mirror="false"
    data-aos-once="true"
    class="flex justify-center gap-5 py-10 align-baseline md:gap-20"
  >
    <a :href="github" target="_blank"
      ><i
        class="text-4xl cursor-pointer text-clrSecondary fa-brands fa-github hover:text-clrAccent"
      ></i>
    </a>
    <a :href="linkedin" target="_blank"
      ><i
        class="text-4xl cursor-pointer text-clrSecondary fa-brands fa-linkedin hover:text-clrAccent"
      ></i
    ></a>
    <a :href="twitter" target="_blank"
      ><i
        class="text-4xl cursor-pointer text-clrSecondary fa-brands fa-twitter hover:text-clrAccent"
      ></i
    ></a>
  </div>
</template>

<script setup>
const twitter = "https://x.com/Alok_Thakur365";
const github = "https://github.com/alok-112";
const linkedin = "https://www.linkedin.com/in/alok-thakur/";
</script>

[warn] --jsx-bracket-same-line is deprecated.
[warn] Ignored unknown option --loglevel=error. Did you mean --log-level?
[warn] Ignored unknown option --stdin.
[warn] --jsx-bracket-same-line is deprecated. [warn] Ignored unknown option
--loglevel=error. Did you mean --log-level? [warn] Ignored unknown option
--stdin. [warn] --jsx-bracket-same-line is deprecated. [warn] Ignored unknown
option --loglevel=error. Did you mean --log-level? [warn] Ignored unknown option
--stdin.
<template>
  <main>
    <section id="masthead" :style="{'min-height': windowHeight + 'px'}">
      <div class="profile">
        <img
          class="image scroll-hidden"
          src="/images/xuyuan_portrait.png"
          alt="A picture of Xuyuan"
        />
        <div class="wrapper scroll-hidden" style="--delay: 250ms">
          <h1 class="title">Hello, I'm Xuyuan.</h1>
          <h3 class="subtitle">
            I'm a student and aspiring software designer currently studying at
            Hwa Chong Institution (JC), Singapore.
          </h3>
        </div>
      </div>

      <Contacts />

      <div class="scroll-wrapper scroll-hidden" style="--delay: 750ms">
        <div class="scroll"></div>
      </div>
    </section>

    <section>
      <a id="experience" class="scroll-id"></a>
      <h2 class="scroll-hidden">Experience</h2>

      <div class="deck">
        <NuxtLink
          class="card card-double scroll-hidden"
          to="/projects/garuda-robotics"
        >
          <img class="image" src="/images/mydronefleets.png" />
          <div class="info">
            <div class="metadata">
              <h4>Internship</h4>
              <h4>2022</h4>
            </div>
            <h3>Garuda Robotics - Airspace management for UAVS</h3>
            <div class="tags">
              <span>Backend</span>
              <span>JavaScript</span>
              <span>OneMap SG</span>
              <span>MongoDB</span>
            </div>
            <SeeMore />
          </div>
        </NuxtLink>
      </div>
    </section>

    <section>
      <a id="projects" class="scroll-id"></a>
      <h2 class="scroll-hidden">Projects</h2>

      <div class="deck">
        <NuxtLink class="card scroll-hidden" to="/projects/musicalrooms">
          <img class="image" src="/images/musicalrooms.png" />

          <div class="info">
            <div class="metadata">
              <h4>Project & Website</h4>
              <h4>2023 - 2024</h4>
            </div>
            <h3>International Youth Science Forum 2024</h3>
            <div class="tags">
              <span>Photography</span>
              <span>Vue/Nuxt</span>
              <span>UI/UX</span>
            </div>
            <SeeMore />
          </div>
        </NuxtLink>

        <NuxtLink class="card scroll-hidden" to="/projects/musicalrooms">
          <img class="image" src="/images/musicalrooms.png" />
          <div class="info">
            <div class="metadata">
              <h4>Web App</h4>
              <h4>2023</h4>
            </div>
            <h3>AITuitionCher - <br />Tuition Assistant for SG Students</h3>
            <div class="tags">
              <span>Vue/Nuxt</span>
              <span>Flask</span>
              <span>GPT3.5</span>
            </div>
            <SeeMore />
          </div>
        </NuxtLink>

        <NuxtLink class="card scroll-hidden" to="/projects/musicalrooms">
          <img class="image" src="/images/musicalrooms.png" />
          <div class="info">
            <div class="metadata">
              <h4>Web App</h4>
              <h4>2023 - 2024</h4>
            </div>
            <h3>Titration! - <br />Teaching Tool for Science Practical</h3>
            <div class="tags">
              <span>ML/AI</span>
              <span>YOLO</span>
              <span>efficientX3D</span>
            </div>
            <SeeMore />
          </div>
        </NuxtLink>

        <NuxtLink class="card scroll-hidden" to="/projects/musicalrooms">
          <img class="image" src="/images/musicalrooms.png" />
          <div class="info">
            <div class="metadata">
              <h4>Mobile App</h4>
              <h4>2021 - 2022</h4>
            </div>
            <h3>MusicalRooms - <br />Educational toolbox for Music Theory</h3>
            <div class="tags">
              <span>iOS</span>
              <span>Swift UI</span>
              <span>UI/UX</span>
            </div>
            <SeeMore />
          </div>
        </NuxtLink>
      </div>
    </section>

    <section class="tech-skills">
      <a id="tech-skills" class="scroll-id"></a>
      <h2 class="scroll-hidden">Tech Skills</h2>

      <div class="scroll-hidden">
        <h3>Programming Languages</h3>
        <div class="badge-list">
          <img
            src="https://img.shields.io/badge/Go-292929?style=for-the-badge&logo=go&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/Swift-292929?style=for-the-badge&logo=swift&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/JavaScript-292929?style=for-the-badge&logo=javascript&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/HTML5-292929?style=for-the-badge&logo=html5&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/CSS3-292929?style=for-the-badge&logo=css3&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/Java-292929?style=for-the-badge&logo=java&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/Kotlin-292929?style=for-the-badge&logo=kotlin&logoColor=white"
          />
        </div>
      </div>

      <div class="scroll-hidden">
        <h3>Tools</h3>
        <div class="badge-list">
          <img
            src="https://img.shields.io/badge/VueJS-292929?style=for-the-badge&logo=vue.js&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/NuxtJS-292929?style=for-the-badge&logo=nuxt.js&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/TailwindCSS-292929?style=for-the-badge&logo=tailwindcss&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/MongoDB-292929?style=for-the-badge&logo=mongodb&logoColor=white"
          />
        </div>
      </div>

      <div class="scroll-hidden">
        <h3>Platforms</h3>
        <div class="badge-list">
          <img
            src="https://img.shields.io/badge/Docker-292929?style=for-the-badge&logo=docker&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/Nginx-292929?style=for-the-badge&logo=nginx&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/Vercel-292929?style=for-the-badge&logo=vercel&logoColor=white"
          />
          <img
            src="https://img.shields.io/badge/Google_Cloud-292929?style=for-the-badge&logo=googlecloud&logoColor=white"
          />
        </div>
      </div>
    </section>

    <a id="academic" class="scroll-id"></a>
    <section>
      <h2 class="scroll-hidden">Academic Qualifications</h2>
      <div class="scroll-hidden">
        <p>
          GCE 'O' Level Equivalent - Secondary 4 Integrated Programme (2022)
        </p>
        <p>Singapore-Cambridge GCE 'O' Level - Higher Chinese (2022)</p>
      </div>
    </section>

    <a id="contact" class="scroll-id"></a>
    <section>
      <h2 class="scroll-hidden">Contact Me</h2>
      <Contacts />
    </section>
  </main>
</template>

<style scoped>
@import '~/assets/css/masthead.css';
@import '~/assets/css/cards.css';
@import '~/assets/css/timeline.css';

main {
  text-align: center;
}
ul {
  list-style: none;
  padding-left: 0;
}

.tech-skills h3 {
  margin: 2rem 0 0.75rem;
}
.badge-list * {
  display: inline-block;
  margin: 0 0.25rem;
}

:not(#masthead) h2 {
  font-weight: semibold;
  font-size: 20px;
  text-transform: uppercase;
  letter-spacing: 0.6rem;
  margin: 7rem 0 3rem;
}
@media screen and (min-width: 800px) {
  :not(#masthead) h2 {
    letter-spacing: 1rem;
    margin: 8.5rem 0 3rem;
  }

  :not(#masthead) .contact {
    gap: 2.125rem;
  }
}
</style>

<script setup>
import EmailIcon from 'vue-material-design-icons/Email.vue';
import {ref, onMounted} from 'vue';

let windowHeight = ref(6000);

onMounted(() => {
  windowHeight.value = window.innerHeight;
});
</script>

<template>
  <main>
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

    <section>
      <h2 class="scroll-hidden">Academic Timeline</h2>

      <div class="timeline">
        <span class="comment right scroll-hidden">2023 - present</span>
        <div class="elm left scroll-hidden">
          <h3>Hwa Chong Junior College</h3>
          <p>
            Subjects offered : Physics (H2), Computing (H2), Math (H2),
            Economics (H2), GP (H1) and PW (H1)
          </p>
        </div>

        <span class="comment left scroll-hidden">2019 - 2022</span>
        <div class="elm right scroll-hidden">
          <h3>Hwa Chong High School</h3>
          <p>
            Subjects offered: Physics, Chemistry, Math, Higher Chinese, English,
            History and Social Studies
          </p>
        </div>

        <span class="comment right scroll-hidden">2016 - 2018</span>
        <div class="elm left scroll-hidden">
          <h3>Nan Hua Primary School</h3>
        </div>

        <span class="comment left scroll-hidden">2013 - 2015</span>
        <div class="elm right scroll-hidden">
          <h3>Rulang Primary School</h3>
        </div>
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
@import "~/assets/css/masthead.css";
@import "~/assets/css/cards.css";
@import "~/assets/css/timeline.css";

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
import EmailIcon from "vue-material-design-icons/Email.vue";
import { ref, onMounted } from "vue";

let windowHeight = ref(6000);

onMounted(() => {
  windowHeight.value = window.innerHeight;
});
</script>

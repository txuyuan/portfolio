<template>
  <main>
    <img
      src="~/assets/images/githubProfile.jpg"
      alt="Xuyuan's Github Profile"
      class="header__image"
    />

    <div class="content">
      <header>
        <h1 class="title">My Programming Adventures</h1>
      </header>

      <p>
        I've been doing programming as a hobby for over 2 years, doing various
        projects and attending programmes. I love the ability to create whatever
        I want, do whatever I want, however I want.
      </p>
      <p>
        For instance, I was unsatisfied with all the free website-creating tools
        on the web, so I spent about a week creating this website! Using various
        tools and programming languages, I can create exactly what I envision.
      </p>

      <h2>TraceTogether Alternative (TTA)</h2>
      <section class="hybrid-para">
        <div class="hybrid-para__text">
          <p>
            My PW project 2021. A product aimed at pointing out the flaws of the
            TraceTogether system and finding ways to solve them. After its
            official conclusion, I decided to do some more work on it in my own
            time. I used it as a testbed and practical example to learn things
            that were related. For instance, since it involved transmitting
            location and contact data, I could test different methods of data
            transmission, using it as a practical dataset.
          </p>
        </div>
        <!-- TODO: replace with Github screenshot -->
        <div class="hybrid-para__image">
          <img src="~/assets/images/ttaCode.jpg" alt="TTA code" />
        </div>
      </section>

      <h2>Swift Accelerator Programme (SAP)</h2>
      <section class="hybrid-para">
        <div class="hybrid-para__text">
          <p>
            An educational programme and gathering place for people interested
            in UI&UX development on iOS. Hosted by Tinkercademy and sponsored by
            Apple and IMDA, I got an opportunity to meet with people of similiar
            interests and learn from people who had been in the industry.
          </p>
        </div>
        <div class="hybrid-para__image">
          <img src="~/assets/images/sapGroup.jpg" alt="SAP group photo" />
        </div>
      </section>

      <section class="hybrid-para">
        <div class="hybrid-para__text">
          <p>
            Our group also created a final product, an app 'MusicalRooms'
            (available on the App Store
            <Link href="https://apps.apple.com/sg/app/musicalrooms/id1597490110"
              >here</Link
            >).
          </p>
          <p>
            This app was created as a toolkit for music theory learners,
            beginners or veterans. We saw that most music theory apps had poor
            interfaces or were paid apps, so we created a simple app with most
            of the basic tools needed for learning music theory, including:
          </p>
          <ul>
            <li>theory exercises</li>
            <li>tuner</li>
            <li>metronome</li>
            <li>recorder</li>
          </ul>
        </div>
        <!-- TODO: mash 2 screens together -->
        <div class="hybrid-para__image">
          <img
            src="~/assets/images/sapProduct.jpg"
            alt="The product of my time at SAP"
          />
        </div>
      </section>

      <h2>Monster Melancholy</h2>

      <section class="hybrid-para">
        <!-- TODO: get actual screenshot -->
        <div class="hybrid-para__text">
          <p>
            Monster Melancholy is a game project started by a friend that I
            found interesting. It's a simple adventure-style game that guides
            the player on a journey through a magical, medieval-style world,
            battling monsters for glory and for resources.
          </p>
          <p>
            I created and continue to maintain the introduction and guide for
            the game, in the form of a website at
            <Link href="https://monster-melancholy.me"
              >monster-melancholy.me</Link
            >. Being my first web project, this is the hook that got me into web
            development
          </p>
        </div>
        <div class="hybrid-para__image">
          <img src="~/assets/images/mmgWebsite.jpg" alt="MMG website code" />
        </div>
      </section>
    </div>
  </main>
</template>

<style scoped>
@import "~/assets/css/document.css";
@import "~/assets/css/portfolio.css";
</style>

<script>
export default {
  head() {
    return {
      title: "My Programming Adventures",
    };
  },
};
</script>

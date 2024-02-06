<template>
  <ul class="contact scroll-hidden">
    <li style="--delay: 0ms">
      <a
        href="mailto:t.xuyuan@gmail.com"
        onclick="javascript:window.open('mailto:t.xuyuan@gmail.com', 'mail');event.preventDefault()"
        target="_blank"
        ><IconMail />Personal&nbsp;Email (preferred)</a
      >
    </li>
    <li style="--delay: 50ms">
      <a
        href="mailto:191519R@student.hci.edu.sg"
        onclick="javascript:window.open('mailto:191519R@student.hci.edu.sg', 'mail');event.preventDefault()"
        target="_blank"
        ><IconMail />Institution&nbsp;Email</a
      >
    </li>
    <li style="--delay: 100ms">
      <a href="https://github.com/txuyuan" target="_blank"
        ><IconGithub />Github</a
      >
    </li>
    <li style="--delay: 150ms">
      <a href="https://www.instagram.com/t.xuyuan/" target="_blank"
        ><IconInstagram />Instagram</a
      >
    </li>
  </ul>
</template>

<style scoped>
.contact {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 1.5rem;
  font-size: 14px;
}
.contact svg {
  margin: 0 0.25rem;
  color: var(--fg);
}
</style>

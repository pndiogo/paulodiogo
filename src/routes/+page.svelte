<script lang="ts">
  import { Linkedin, ScrollText, Send } from 'lucide-svelte';

  const iconStrokeWidth = 1.5;
</script>

<svelte:head>
  <link rel="preload" href="/videos/bkg-video.webm" as="style" />
  <link rel="preload" href="/videos/bkg-video.mp4" as="video" />
</svelte:head>

<section class="main bg-accent">
  <video
    autoplay
    loop
    muted
    playsinline
    class="object-cover w-full h-full max-h-screen"
  >
    <source src="/videos/bkg-video.webm" type="video/webm" />
    <source src="/videos/bkg-video.mp4" type="video/mp4" />
    <track kind="captions" />
  </video>
  <div class="bkg-overlay w-full h-full mix-blend-overlay"></div>
  <article
    class="profile grid grid-cols-5 bg-white shadow-2xl overflow-hidden rounded-md max-w-lg md:max-w-2xl lg:max-w-4xl z-10 m-6"
  >
    <div class="profile-image col-span-2 hidden lg:block">
      <picture class="block w-full h-full">
        <source srcset="/images/profile.webp" type="image/webp" />
        <img
          class="object-cover w-full h-full"
          src="/images/profile.jpg"
          alt="Profile"
        />
      </picture>
    </div>
    <div class="profile-content col-span-5 lg:col-span-3 px-8 pt-5 pb-8">
      <div class="flex items-center gap-4">
        <picture class="hidden sm:block lg:hidden w-40 h-full">
          <source srcset="/images/profile.webp" type="image/webp" />
          <img
            class="object-cover w-full h-full rounded-sm"
            src="/images/profile.jpg"
            alt="Profile"
          />
        </picture>
        <div>
          <h1 class="text-5xl font-bold lg:leading-snug mb-2 lg:mb-0">
            Paulo Diogo
          </h1>
          <h2 class="text-3xl leading-snug text-zinc-800">Web Developer</h2>
        </div>
      </div>
      <div class="flex align-middle gap-4 my-4">
        <a
          href="https://linkedin.com/in/pndiogo"
          target="_blank"
          class="text-accent hover:text-black"
          ><Linkedin
            strokeWidth={iconStrokeWidth}
            class="transition-all motion-reduce:transition-none motion-reduce:hover:transform-none"
          /></a
        >
        <a
          href="https://flowcv.com/resume/0o3gclfuss"
          target="_blank"
          class="text-accent hover:text-black"
          ><ScrollText
            strokeWidth={iconStrokeWidth}
            class="transition-all motion-reduce:transition-none motion-reduce:hover:transform-none"
          /></a
        >
        <a
          href="https://tally.so/r/mYaWYv"
          target="_blank"
          class="text-accent hover:text-black"
          ><Send
            strokeWidth={iconStrokeWidth}
            class="transition-all motion-reduce:transition-none motion-reduce:hover:transform-none"
          /></a
        >
      </div>
      <p class="leading-normal my-8">
        Passionate, goal-oriented self-taught developer committed to clean code,
        industry best practices, and innovation. Detail-oriented with a
        proactive problem-solving approach, I bring motivation, effective
        communication, and a dedication to continuous learning for collaborative
        success in dynamic IT environments.
      </p>
      <div class="flex flex-col sm:flex-row items-start sm:items-center gap-4">
        <a
          href="https://flowcv.com/resume/0o3gclfuss"
          target="_blank"
          class="flex items-center gap-2 bg-accent hover:bg-black text-white rounded-sm px-4 py-2 transition motion-reduce:transition-none motion-reduce:hover:transform-none"
          ><ScrollText strokeWidth={iconStrokeWidth} size={20} />Download CV</a
        >
        <a
          href="https://tally.so/r/mYaWYv"
          target="_blank"
          class="flex items-center gap-2 bg-zinc-800 hover:bg-black text-white rounded-sm px-4 py-2 transition motion-reduce:transition-none motion-reduce:hover:transform-none"
          ><Send strokeWidth={iconStrokeWidth} size={20} />
          Send me a message
        </a>
      </div>
    </div>
  </article>
</section>
<a
  class="fixed bottom-1 right-4 text-white text-sm opacity-50 hover:opacity-100 transition motion-reduce:transition-none motion-reduce:hover:transform-none"
  href="https://www.pexels.com/video/waves-rushing-and-splashing-to-the-shore-1409899/"
  target="_blank">Video by Michal Marek</a
>

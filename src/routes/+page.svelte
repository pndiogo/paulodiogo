<svelte:head>
  <link rel="preload" href="/videos/bkg-video.webm" as="style" />
  <link rel="preload" href="/videos/bkg-video.mp4" as="video" />
</svelte:head>

<section class="main">
  <video autoplay loop muted playsinline class="video-player">
    <source src="/videos/bkg-video.webm" type="video/webm" />
    <source src="/videos/bkg-video.mp4" type="video/mp4" />
    <track kind="captions" />
  </video>
  <p>Hello</p>
</section>

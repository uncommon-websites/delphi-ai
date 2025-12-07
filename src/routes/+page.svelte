<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import Features from "$lib/components/Features.svelte";
  import Demo from "$lib/components/Demo.svelte";
  import Trust from "$lib/components/Trust.svelte";
  import UseCases from "$lib/components/UseCases.svelte";
  import Timeline from "$lib/components/Timeline.svelte";
  import CTA from "$lib/components/CTA.svelte";
  import Footer from "$lib/components/Footer.svelte";
  
  let y = 0;
</script>

<svelte:window bind:scrollY={y} />

<main class="bg-cream-50 min-h-screen">
  <Header scrolled={y > 50} />
  <Hero />
  <Features />
  <Demo />
  <Trust />
  <UseCases />
  <Timeline />
  <CTA />
  <Footer />
</main>


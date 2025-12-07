<script>
  export let scrolled = false;
</script>

<header class="fixed top-0 left-0 w-full z-50 transition-all duration-300 {scrolled ? 'bg-cream-50/90 backdrop-blur-md py-3 shadow-sm' : 'bg-transparent py-5'}">
  <div class="max-w-[1400px] mx-auto px-6 flex items-center justify-between">
    <!-- Left Nav -->
    <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-cream-900/80">
      <a href="#industries" class="hover:text-cream-900 transition-colors">Industries</a>
      <a href="#resources" class="hover:text-cream-900 transition-colors">Resources</a>
      <a href="#pricing" class="hover:text-cream-900 transition-colors">Pricing</a>
      <a href="#immortal" class="hover:text-cream-900 transition-colors">Immortal</a>
    </nav>

    <!-- Logo -->
    <div class="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2">
      <a href="/" class="block text-cream-900">
        <svg width="40" height="24" viewBox="0 0 40 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <!-- Stylized >E Logo -->
          <path d="M12 4L20 12L12 20" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M28 4H20" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M28 12H20" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M28 20H20" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
      </a>
    </div>

    <!-- Right Nav -->
    <div class="flex items-center gap-6">
      <a href="#explore" class="hidden md:block text-sm font-medium text-cream-900/80 hover:text-cream-900 transition-colors">Explore</a>
      <a href="#signin" class="hidden md:block text-sm font-medium text-cream-900/80 hover:text-cream-900 transition-colors">Sign in</a>
      <a href="#start" class="bg-[#1C1917] text-white px-5 py-2.5 rounded-full text-sm font-medium hover:bg-black/80 transition-colors">Get Started</a>
    </div>
  </div>
</header>

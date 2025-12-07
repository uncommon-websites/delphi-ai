<script>
  const experts = [
    {
      name: "Sam Feldt",
      role: "Musician",
      image: "https://images.unsplash.com/photo-1500648767791-00dcc994a43e?q=80&w=1000&auto=format&fit=crop",
      color: "from-orange-600/60 to-red-600/60"
    },
    {
      name: "Brian Halligan",
      role: "Executive",
      image: "https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?q=80&w=1000&auto=format&fit=crop",
      color: "from-red-600/60 to-orange-700/60"
    },
    {
      name: "Vanessa Van Edwards",
      role: "Behavioral Scientist",
      image: "https://images.unsplash.com/photo-1544005313-94ddf0286df2?q=80&w=1000&auto=format&fit=crop",
      color: "from-orange-500/60 to-red-500/60"
    },
    {
      name: "Andrew Huberman",
      role: "Neuroscientist",
      image: "https://images.unsplash.com/photo-1560250097-0b93528c311a?q=80&w=1000&auto=format&fit=crop",
      color: "from-red-500/60 to-orange-600/60"
    },
    {
      name: "Lex Fridman",
      role: "Podcaster",
      image: "https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?q=80&w=1000&auto=format&fit=crop",
      color: "from-orange-700/60 to-red-700/60"
    }
  ];
</script>

<section class="pt-32 pb-20 overflow-hidden">
  <div class="max-w-[1400px] mx-auto px-6 text-center">
    
    <a href="#library" class="inline-flex items-center gap-2 text-xs font-medium text-[#E85D3E] mb-8 hover:opacity-80 transition-opacity group">
      The Library of Minds — the first interactive podcast
      <span class="group-hover:translate-x-0.5 transition-transform">
        <svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M2.5 6H9.5M9.5 6L6 2.5M9.5 6L6 9.5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
      </span>
    </a>

    <h1 class="text-6xl md:text-7xl lg:text-8xl font-serif text-cream-900 mb-6 leading-[1.1] tracking-tight">
      Create Your Digital Self
    </h1>

    <p class="text-lg md:text-xl text-cream-900/60 max-w-2xl mx-auto mb-10 leading-relaxed font-light">
      Your Mind. Your Model. Your Rules.<br>
      Answer Questions & Connect 24/7 In Your Voice
    </p>

    <div class="flex items-center justify-center gap-4 mb-20">
      <button class="bg-[#1C1917] text-white px-8 py-3.5 rounded-full font-medium hover:bg-black/90 transition-colors">
        Create My Delphi
      </button>
      <button class="bg-transparent border border-cream-900/20 text-cream-900 px-8 py-3.5 rounded-full font-medium hover:bg-cream-900/5 transition-colors">
        Explore Experts
      </button>
    </div>

  </div>

  <!-- Carousel -->
  <div class="w-full overflow-x-auto pb-10 hide-scrollbar px-6">
    <div class="flex gap-6 w-max mx-auto px-6">
      {#each experts as expert}
        <div class="relative w-[280px] h-[380px] rounded-2xl overflow-hidden group cursor-pointer flex-shrink-0">
          <img src={expert.image} alt={expert.name} class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105 filter sepia-[0.2] contrast-110" />
          
          <!-- Gradient Overlay -->
          <div class="absolute inset-0 bg-gradient-to-t {expert.color} mix-blend-multiply opacity-60 group-hover:opacity-70 transition-opacity duration-300"></div>
          
          <!-- Bottom Gradient for text readability -->
          <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-transparent to-transparent"></div>

          <div class="absolute bottom-0 left-0 w-full p-6 text-white text-center z-10">
            <h3 class="font-serif text-xl mb-1">{expert.name}</h3>
            <p class="text-[10px] font-bold uppercase tracking-widest opacity-80">{expert.role}</p>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>

<style>
  .hide-scrollbar::-webkit-scrollbar {
    display: none;
  }
  .hide-scrollbar {
    -ms-overflow-style: none;
    scrollbar-width: none;
  }
</style>

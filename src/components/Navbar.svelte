<script>
  import avatar from '$lib/image/pic.jpeg';
  let isMobileMenuOpen = false;

  function toggleMobileMenu() {
    isMobileMenuOpen = !isMobileMenuOpen;
  }
</script>

<style>
  .mobile-menu {
    max-height: 0;
    overflow: hidden;
    transition: max-height 2.0s ease;
  }

  .mobile-menu.active {
    max-height: 1000px; /* Sesuaikan dengan tinggi maksimum menu */
    transition: max-height 2.0s ease;
  }
</style>

<nav class="px-12 py-3 bg-stone-200 sm:px-28 top-0 sticky z-50">
  <div class="flex items-center justify-between">
    <div class="flex items-center">
      <h1 class="text-black text-2xl ml-2 font-medium">Shayna.</h1>
    </div>
    <div class="md:hidden">
      <button class="text-black hover:text-stone-400" on:click={toggleMobileMenu}>
        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
        </svg>
      </button>
    </div>
    <div class="hidden md:flex space-x-4">
      <a href="/" class="text-black hover:text-stone-400">Home</a>
      <a href="/start" class="text-black hover:text-stone-400">Start</a>
      <a href="/browse" class="text-black hover:text-stone-400">Browse</a>
      <a href="/pricing" class="text-black hover:text-stone-400">Pricing</a>
      <a href="/story" class="text-black hover:text-stone-400">Story</a>
    </div>
    <div class="relative flex items-center">
      <img src={avatar} alt="avatar" class="w-10 h-10 object-cover rounded-full">
    </div>
  </div>
  <div class="mobile-menu mt-2 md:hidden" class:active={isMobileMenuOpen}>
    <a href="/" class="block text-black hover:text-stone-400">Home</a>
    <a href="/start" class="block text-black hover:text-stone-400">Start</a>
    <a href="/browse" class="block text-black hover:text-stone-400">Browse</a>
    <a href="/pricing" class="block text-black hover:text-stone-400">Pricing</a>
    <a href="/story" class="block text-black hover:text-stone-400">Story</a>
  </div>
</nav>

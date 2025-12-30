<script lang="ts">
  import Button from './Button.svelte';
  
  let isMenuOpen = false;
</script>

<nav class="fixed top-0 left-0 right-0 z-50 bg-cream/90 backdrop-blur-sm border-b border-gray-200/50">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex justify-between items-center h-20">
      <!-- Logo -->
      <div class="flex-shrink-0 flex items-center">
        <a href="/" class="flex items-center gap-2">
          <!-- Glimkin Logo Icon -->
          <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M16 28C22.6274 28 28 22.6274 28 16C28 9.37258 22.6274 4 16 4C9.37258 4 4 9.37258 4 16C4 22.6274 9.37258 28 16 28Z" fill="oklch(0.592 0.249 0.584)"/>
            <ellipse cx="12" cy="14" rx="2" ry="3" fill="white"/>
            <ellipse cx="20" cy="14" rx="2" ry="3" fill="white"/>
            <path d="M11 20C11 20 13 22 16 22C19 22 21 20 21 20" stroke="white" stroke-width="2" stroke-linecap="round"/>
            <path d="M8 10C8 10 10 8 12 8" stroke="oklch(0.592 0.249 0.584)" stroke-width="1.5" stroke-linecap="round"/>
            <path d="M24 10C24 10 22 8 20 8" stroke="oklch(0.592 0.249 0.584)" stroke-width="1.5" stroke-linecap="round"/>
          </svg>
          <span class="font-bold text-xl tracking-tight">Glimkin</span>
        </a>
      </div>

      <!-- Desktop Navigation -->
      <div class="hidden md:flex items-center space-x-8">
        <a href="#" class="text-sm font-medium hover:text-primary-brand transition-colors">Collections</a>
        <a href="#" class="text-sm font-medium hover:text-primary-brand transition-colors">How It Works</a>
        <a href="#" class="text-sm font-medium hover:text-primary-brand transition-colors">Community</a>
      </div>

      <!-- Right Side -->
      <div class="hidden md:flex items-center space-x-6">
        <a href="#" class="text-sm font-medium hover:text-primary-brand transition-colors">About</a>
        <a href="#" class="text-sm font-medium hover:text-primary-brand transition-colors">FAQ</a>
        <Button href="#" className="!py-2 !px-4 !text-sm">Back a Plush &rarr;</Button>
      </div>

      <!-- Mobile menu button -->
      <div class="md:hidden flex items-center">
        <button on:click={() => isMenuOpen = !isMenuOpen} class="text-gray-600 hover:text-gray-900 focus:outline-none">
          <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>
    </div>
  </div>
</nav>

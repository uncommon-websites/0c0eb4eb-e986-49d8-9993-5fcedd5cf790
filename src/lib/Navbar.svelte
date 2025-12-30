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
          <!-- Glimkin Logo -->
          <svg width="32" height="30" viewBox="0 0 112 106" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M111.712 30.2285V0C92.366 0 73.5034 6.52934 59.961 17.8952L56.3336 20.7972L52.7062 17.8952C38.922 6.52934 20.3013 0 0.955078 0V30.2285C0.955078 38.4506 3.85704 46.1891 8.6936 52.7184C3.85704 59.2478 0.955078 66.9863 0.955078 75.2085V105.437C20.3013 105.437 39.1639 98.9076 52.7062 87.5417L56.3336 84.6397C46.9023 79.0777 41.0985 69.1627 41.0985 58.0387V47.3983C41.0985 36.516 46.9023 26.3592 56.3336 20.7972C65.7649 26.3592 71.5688 36.516 71.5688 47.3983V58.0387C71.5688 68.9209 65.7649 79.0777 56.3336 84.6397L59.961 87.5417C73.7452 98.9076 92.366 105.437 111.712 105.437V75.2085C111.712 66.9863 108.81 59.2478 103.974 52.7184C108.81 46.1891 111.712 38.4506 111.712 30.2285Z" fill="#201B21"/>
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

<script>
  import { onMount } from 'svelte';

  const images = [
    "https://images.unsplash.com/photo-1490481651871-ab68de25d43d?q=80&w=400&auto=format&fit=crop", // Fashion shopping
    "https://images.unsplash.com/photo-1445205170230-053b83016050?q=80&w=400&auto=format&fit=crop", // Clothing rack
    "https://images.unsplash.com/photo-1591047139829-d91aecb6caea?q=80&w=400&auto=format&fit=crop", // Sneakers
    "https://images.unsplash.com/photo-1558769132-cb1aea1f1c9a?q=80&w=400&auto=format&fit=crop", // Handbag
    "https://images.unsplash.com/photo-1523381210434-271e8be1f52b?q=80&w=400&auto=format&fit=crop"  // Clothing items
  ];

  let showCookieBanner = $state(true);
</script>

<div class="font-sans text-[#111] antialiased bg-white selection:bg-black selection:text-white">
  <!-- Header -->
  <header class="fixed top-0 left-0 w-full z-50 flex justify-between items-center px-6 py-5 bg-white/90 backdrop-blur-sm">
    <div class="flex items-center gap-3">
      <svg width="40" height="27" viewBox="0 0 117 78" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path fill-rule="evenodd" clip-rule="evenodd" d="M83.0101 48.3334H67.6809C65.1171 48.3334 62.6584 49.3518 60.8454 51.1647L56.8415 55.1687C55.0285 56.9817 52.5698 58 50.0059 58H34.6768C26.6686 58 20.1768 51.5081 20.1768 43.5C20.1768 35.4919 26.6686 29 34.6768 29H50.0059C52.5698 29 55.0285 27.9817 56.8415 26.1687L60.8454 22.1647C62.6584 20.3518 65.1171 19.3334 67.6809 19.3334H83.0101C91.0182 19.3334 97.5101 25.8253 97.5101 33.8334C97.5101 41.8415 91.0182 48.3334 83.0101 48.3334ZM67.6809 29C65.1171 29 62.6584 30.0184 60.8454 31.8314L56.8415 35.8353C55.0285 37.6483 52.5698 38.6667 50.0059 38.6667H34.6768C32.0073 38.6667 29.8434 40.8306 29.8434 43.5C29.8434 46.1695 32.0073 48.3334 34.6768 48.3334H50.0059C52.5698 48.3334 55.0285 47.315 56.8415 45.502L60.8454 41.4981C62.6584 39.6851 65.1171 38.6667 67.6809 38.6667H83.0101C85.6795 38.6667 87.8434 36.5028 87.8434 33.8334C87.8434 31.1639 85.6795 29 83.0101 29H67.6809Z" fill="black"/>
        <path fill-rule="evenodd" clip-rule="evenodd" d="M83.0104 67.6667H67.6813C65.1174 67.6667 62.6587 68.6851 60.8457 70.498L56.8418 74.502C55.0288 76.3149 52.5701 77.3333 50.0062 77.3333H34.6771C15.9914 77.3333 0.84375 62.1857 0.84375 43.5C0.84375 24.8143 15.9914 9.66667 34.6771 9.66667H50.0062C52.5701 9.66667 55.0288 8.64828 56.8418 6.8353L60.8457 2.83129C62.6587 1.01846 65.1174 0 67.6813 0H83.0104C101.696 0 116.844 15.1477 116.844 33.8333C116.844 52.519 101.696 67.6667 83.0104 67.6667ZM67.6813 9.66667C65.1174 9.66667 62.6587 10.6851 60.8457 12.498L56.8418 16.502C55.0288 18.3149 52.5701 19.3333 50.0062 19.3333H34.6771C21.3302 19.3333 10.5104 30.1532 10.5104 43.5C10.5104 56.8468 21.3302 67.6667 34.6771 67.6667H50.0062C52.5701 67.6667 55.0288 66.6483 56.8418 64.8353L60.8457 60.8314C62.6587 59.0184 65.1174 58 67.6813 58H83.0104C96.3572 58 107.177 47.1801 107.177 33.8333C107.177 20.4866 96.3572 9.66667 83.0104 9.66667H67.6813Z" fill="black"/>
      </svg>
      <span class="text-xl font-medium tracking-tight">16commerce</span>
    </div>
    <nav class="hidden md:flex items-center gap-8 text-sm font-medium">
      <a href="#platform" class="hover:opacity-70 transition-opacity">Platform</a>
      <a href="#benefits" class="hover:opacity-70 transition-opacity">Benefits</a>
      <a href="#integration" class="hover:opacity-70 transition-opacity">Integration</a>
      <a href="#contact" class="hover:opacity-70 transition-opacity">Contact</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="pt-40 pb-20 px-6 max-w-[1400px] mx-auto">
    <div class="max-w-4xl mb-24">
      <h1 class="text-6xl md:text-7xl font-medium tracking-tight leading-[1.1] mb-8">
        Turn resellers into<br>repeat buyers
      </h1>
      <div class="flex flex-col md:flex-row justify-between items-start md:items-end gap-8">
        <p class="text-lg md:text-xl max-w-md leading-relaxed text-gray-800">
          Asset-light P2P marketplaces that help SEA fashion brands monetize past sales and capture the $50B resale market.
        </p>
        <button class="bg-black text-white px-6 py-3 text-sm font-medium rounded-sm hover:bg-gray-800 transition-colors">
          Get started
        </button>
      </div>
    </div>

    <!-- Hero Images Grid -->
    <div class="grid grid-cols-2 md:grid-cols-5 gap-4">
      {#each images as src, i}
        <div class="aspect-[3/4] overflow-hidden bg-gray-100 rounded-sm">
          <img {src} alt="Fashion item {i}" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
        </div>
      {/each}
    </div>
  </section>

  <!-- Floating Images Section -->
  <section class="py-32 px-6 max-w-[1400px] mx-auto relative min-h-[800px]">
    <div class="absolute inset-0 flex items-center justify-center pointer-events-none z-10">
      <h2 class="text-2xl md:text-3xl font-medium text-center max-w-2xl leading-snug bg-white/80 backdrop-blur-sm p-4 rounded-xl">
        Enable your customers to buy and sell pre-loved fashion seamlessly, without holding any inventory.
      </h2>
    </div>

    <!-- Scattered Images with 'List for resale' -->
    <div class="relative w-full h-full min-h-[800px]">
      <!-- Image 1: Clothing rack (Left) -->
      <div class="absolute top-20 left-[10%] w-64 aspect-[3/4]">
        <img src={images[1]} alt="Fashion items" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <div class="w-3 h-3 bg-white rounded-full mx-auto mb-2 animate-pulse"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">List for resale</button>
        </div>
      </div>

      <!-- Image 2: Handbag (Center Top) -->
      <div class="absolute top-0 left-[45%] w-56 aspect-[3/4]">
        <img src={images[3]} alt="Designer handbag" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/3 left-1/3">
             <div class="w-3 h-3 bg-white rounded-full mb-2 animate-pulse"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">List for resale</button>
        </div>
      </div>

       <!-- Image 3: Clothing items (Right Top) -->
      <div class="absolute top-40 right-[5%] w-80 aspect-video">
        <img src={images[4]} alt="Fashion collection" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute bottom-1/3 right-1/3">
             <div class="w-3 h-3 bg-white rounded-full mb-2 animate-pulse ml-auto"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">List for resale</button>
        </div>
      </div>

      <!-- Image 4: Fashion shopping (Left Bottom) -->
      <div class="absolute bottom-20 left-[5%] w-56 aspect-[3/4]">
        <img src={images[0]} alt="Shopping bags" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">List for resale</button>
        </div>
      </div>

      <!-- Image 5: Sneakers (Center Bottom) -->
      <div class="absolute bottom-0 left-[35%] w-48 aspect-[3/4]">
        <img src={images[2]} alt="Sneakers" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">List for resale</button>
        </div>
      </div>
    </div>
  </section>

  <!-- Dark Section 1: Credit Loop Retention -->
  <section class="bg-[#111] text-white py-32 px-6" id="platform">
    <div class="max-w-[1400px] mx-auto">
      <div class="flex flex-col md:flex-row justify-between items-start mb-20 gap-8">
        <h2 class="text-4xl md:text-5xl font-medium tracking-tight max-w-xl">
          Credit-loop retention<br>that drives repeat purchases
        </h2>
        <p class="text-gray-400 text-lg max-w-md leading-relaxed">
          When customers resell, they earn store credit. This keeps them coming back to your brand instead of losing them to third-party resale platforms.
        </p>
      </div>

      <!-- Interactive Box -->
      <div class="w-full aspect-video bg-[#1a1a1a] rounded-sm mb-16 flex items-center justify-center relative overflow-hidden group">
        <div class="flex flex-col items-center gap-6">
          <div class="text-3xl md:text-5xl font-light tracking-tight text-white/90">
            Sell → Credit → Buy Again
          </div>
          <div class="flex items-center gap-4">
            <div class="w-3 h-3 bg-primary-500 rounded-full animate-pulse"></div>
            <div class="text-primary-500 text-sm font-medium">Continuous customer loop</div>
          </div>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-12 border-t border-white/10 pt-12">
        <div>
          <h3 class="text-lg font-medium mb-3">Zero inventory risk</h3>
          <p class="text-gray-400 leading-relaxed">P2P model means you never hold resale inventory.</p>
        </div>
        <div>
          <h3 class="text-lg font-medium mb-3">Commission-based revenue</h3>
          <p class="text-gray-400 leading-relaxed">Earn on every resale transaction with no upfront costs.</p>
        </div>
        <div>
          <h3 class="text-lg font-medium mb-3">Customer retention</h3>
          <p class="text-gray-400 leading-relaxed">Keep customers in your ecosystem with store credit incentives.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Dark Section 2: Asset-Light Infrastructure -->
  <section class="bg-[#111] text-white py-32 px-6 border-t border-white/5">
    <div class="max-w-[1400px] mx-auto">
      <div class="flex flex-col md:flex-row justify-between items-start mb-20 gap-8">
        <h2 class="text-4xl md:text-5xl font-medium tracking-tight">
          Asset-light infrastructure<br>built for scale
        </h2>
        <p class="text-gray-400 text-lg max-w-md leading-relaxed">
          Launch your resale marketplace without warehouses, logistics teams, or inventory management. We handle the platform, you focus on your brand.
        </p>
      </div>

      <!-- Interactive Box -->
      <div class="w-full aspect-[2/1] bg-[#1a1a1a] rounded-sm flex items-center justify-center">
         <div class="grid grid-cols-3 gap-8 text-center">
          <div>
            <div class="text-4xl md:text-6xl font-light text-primary-500 mb-2">0%</div>
            <div class="text-sm text-gray-400">Inventory held</div>
          </div>
          <div>
            <div class="text-4xl md:text-6xl font-light text-primary-500 mb-2">100%</div>
            <div class="text-sm text-gray-400">Commission model</div>
          </div>
          <div>
            <div class="text-4xl md:text-6xl font-light text-primary-500 mb-2">$50B</div>
            <div class="text-sm text-gray-400">Market opportunity</div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Light Gray Section -->
  <section class="bg-[#f5f5f5] py-24 px-6" id="benefits">
    <div class="max-w-[1400px] mx-auto grid grid-cols-1 md:grid-cols-3 gap-12">
      <div>
        <h3 class="text-lg font-medium mb-3 text-[#111]">Recapture lost customers</h3>
        <p class="text-gray-600 leading-relaxed">Stop losing customers to third-party resale platforms like Carousell and Shopee.</p>
      </div>
      <div>
        <h3 class="text-lg font-medium mb-3 text-[#111]">Increase lifetime value</h3>
        <p class="text-gray-600 leading-relaxed">Turn one-time buyers into repeat customers through the credit-loop system.</p>
      </div>
      <div>
        <h3 class="text-lg font-medium mb-3 text-[#111]">New revenue stream</h3>
        <p class="text-gray-600 leading-relaxed">Monetize past sales with commission-based resale transactions.</p>
      </div>
    </div>
  </section>

  <!-- Built for SEA Fashion Brands -->
  <section class="bg-[#f0f0f0] py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <div class="mb-16">
        <h2 class="text-4xl md:text-5xl font-medium tracking-tight mb-6 text-[#111]">
          Built for SEA fashion brands
        </h2>
        <p class="text-gray-600 text-lg max-w-2xl leading-relaxed">
          16commerce is designed specifically for Southeast Asian fashion brands who want to capture the resale market without the complexity of traditional recommerce platforms.
        </p>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-start">
        <!-- Visual -->
        <div class="bg-[#111] aspect-video rounded-xl flex items-center justify-center relative overflow-hidden perspective-1000">
           <!-- Abstract Marketplace Flow -->
           <div class="relative w-full h-full flex items-center justify-center p-8">
              <div class="grid grid-cols-3 gap-4 w-full max-w-md">
                {#each [0, 1, 2, 3, 4, 5] as i}
                  <div 
                    class="aspect-square border border-white/30 bg-white/5 backdrop-blur-sm rounded-sm transition-all duration-500 hover:border-primary-500 hover:bg-primary-500/10"
                    style="animation-delay: {i * 0.1}s"
                  ></div>
                {/each}
              </div>
           </div>
        </div>

        <!-- List -->
        <div class="space-y-12 pt-4">
          <div class="group cursor-pointer">
            <h3 class="text-xl font-medium mb-3 text-[#111]">Shopify integration</h3>
            <p class="text-gray-600 leading-relaxed">Seamlessly integrate with your existing Shopify store. Launch your resale marketplace in days, not months.</p>
          </div>
          <div class="group cursor-pointer opacity-40 hover:opacity-100 transition-opacity">
            <h3 class="text-xl font-medium mb-3 text-[#111]">No logistics headaches</h3>
            <p class="text-gray-600 leading-relaxed">P2P model means customers handle shipping directly. You focus on your brand, not warehousing.</p>
          </div>
          <div class="group cursor-pointer opacity-40 hover:opacity-100 transition-opacity">
            <h3 class="text-xl font-medium mb-3 text-[#111]">SEA-optimized</h3>
            <p class="text-gray-600 leading-relaxed">Built for Southeast Asian markets with local payment methods, languages, and shopping behaviors in mind.</p>
          </div>

          <div class="flex gap-4 pt-8">
             <button class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center text-gray-400 hover:border-gray-800 hover:text-gray-800 transition-colors">←</button>
             <button class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center text-gray-400 hover:border-gray-800 hover:text-gray-800 transition-colors">→</button>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Fast to Launch -->
  <section class="bg-[#fffcf8] py-32 px-6" id="integration">
    <div class="max-w-[1400px] mx-auto">
      <h2 class="text-4xl md:text-5xl font-medium tracking-tight mb-20 text-[#111]">
        Launch in days, not months
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
        <!-- Card 1 -->
        <div>
          <div class="w-14 h-14 bg-[#111] text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3" />
            </svg>
          </div>
          <h3 class="text-lg font-medium mb-3 text-[#111]">Shopify partner integration</h3>
          <p class="text-gray-600 leading-relaxed">Connect through Shopify partner channels with minimal setup required.</p>
        </div>

        <!-- Card 2 -->
        <div>
          <div class="w-14 h-14 bg-[#111] text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 18.75a60.07 60.07 0 0 1 15.797 2.101c.727.198 1.453-.342 1.453-1.096V18.75M3.75 4.5v.75A.75.75 0 0 1 3 6h-.75m0 0v-.375c0-.621.504-1.125 1.125-1.125H20.25M2.25 6v9m18-10.5v.75c0 .414.336.75.75.75h.75m-1.5-1.5h.375c.621 0 1.125.504 1.125 1.125v9.75c0 .621-.504 1.125-1.125 1.125h-.375m1.5-1.5H21a.75.75 0 0 0-.75.75v.75m0 0H3.75m0 0h-.375a1.125 1.125 0 0 1-1.125-1.125V15m1.5 1.5v-.75A.75.75 0 0 0 3 15h-.75M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Zm3 0h.008v.008H18V10.5Zm-12 0h.008v.008H6V10.5Z" />
            </svg>
          </div>
          <h3 class="text-lg font-medium mb-3 text-[#111]">Zero-inventory model</h3>
          <p class="text-gray-600 leading-relaxed">Commission-based revenue with no upfront costs or inventory risks.</p>
        </div>

        <!-- Card 3 -->
        <div>
          <div class="w-14 h-14 bg-[#111] text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 3v11.25A2.25 2.25 0 0 0 6 16.5h2.25M3.75 3h-1.5m1.5 0h16.5m0 0h1.5m-1.5 0v11.25A2.25 2.25 0 0 1 18 16.5h-2.25m-7.5 0h7.5m-7.5 0-1 3m8.5-3 1 3m0 0 .5 1.5m-.5-1.5h-9.5m0 0-.5 1.5m.75-9 3-3 2.148 2.148A12.061 12.061 0 0 1 16.5 7.605" />
            </svg>
          </div>
          <h3 class="text-lg font-medium mb-3 text-[#111]">Scale with confidence</h3>
          <p class="text-gray-600 leading-relaxed">Asset-light infrastructure grows with your business automatically.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA Banner -->
  <section class="px-6 py-12" id="contact">
    <div class="max-w-[1400px] mx-auto border border-gray-100 rounded-xl p-8 md:p-12 flex flex-col md:flex-row justify-between items-center gap-8 bg-white shadow-sm">
      <div class="flex items-center gap-6">
        <div class="flex gap-1 h-8">
           <div class="w-2 bg-black h-full"></div>
           <div class="w-2 bg-black h-full"></div>
           <div class="w-2 bg-black h-full"></div>
           <div class="w-2 bg-primary-500 h-full"></div>
        </div>
        <h2 class="text-2xl md:text-3xl font-medium tracking-tight">Ready to capture the resale market?</h2>
      </div>
      <button class="bg-black text-white px-8 py-3 text-sm font-medium rounded-sm hover:bg-gray-800 transition-colors whitespace-nowrap">
        Get started today
      </button>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-white pt-20 pb-10 px-6 border-t border-gray-100">
    <div class="max-w-[1400px] mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-12 md:gap-24 mb-20">
        <div class="col-span-1 md:col-span-2">
          <div class="flex items-center gap-3 mb-2">
            <svg width="40" height="27" viewBox="0 0 117 78" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd" clip-rule="evenodd" d="M83.0101 48.3334H67.6809C65.1171 48.3334 62.6584 49.3518 60.8454 51.1647L56.8415 55.1687C55.0285 56.9817 52.5698 58 50.0059 58H34.6768C26.6686 58 20.1768 51.5081 20.1768 43.5C20.1768 35.4919 26.6686 29 34.6768 29H50.0059C52.5698 29 55.0285 27.9817 56.8415 26.1687L60.8454 22.1647C62.6584 20.3518 65.1171 19.3334 67.6809 19.3334H83.0101C91.0182 19.3334 97.5101 25.8253 97.5101 33.8334C97.5101 41.8415 91.0182 48.3334 83.0101 48.3334ZM67.6809 29C65.1171 29 62.6584 30.0184 60.8454 31.8314L56.8415 35.8353C55.0285 37.6483 52.5698 38.6667 50.0059 38.6667H34.6768C32.0073 38.6667 29.8434 40.8306 29.8434 43.5C29.8434 46.1695 32.0073 48.3334 34.6768 48.3334H50.0059C52.5698 48.3334 55.0285 47.315 56.8415 45.502L60.8454 41.4981C62.6584 39.6851 65.1171 38.6667 67.6809 38.6667H83.0101C85.6795 38.6667 87.8434 36.5028 87.8434 33.8334C87.8434 31.1639 85.6795 29 83.0101 29H67.6809Z" fill="black"/>
              <path fill-rule="evenodd" clip-rule="evenodd" d="M83.0104 67.6667H67.6813C65.1174 67.6667 62.6587 68.6851 60.8457 70.498L56.8418 74.502C55.0288 76.3149 52.5701 77.3333 50.0062 77.3333H34.6771C15.9914 77.3333 0.84375 62.1857 0.84375 43.5C0.84375 24.8143 15.9914 9.66667 34.6771 9.66667H50.0062C52.5701 9.66667 55.0288 8.64828 56.8418 6.8353L60.8457 2.83129C62.6587 1.01846 65.1174 0 67.6813 0H83.0104C101.696 0 116.844 15.1477 116.844 33.8333C116.844 52.519 101.696 67.6667 83.0104 67.6667ZM67.6813 9.66667C65.1174 9.66667 62.6587 10.6851 60.8457 12.498L56.8418 16.502C55.0288 18.3149 52.5701 19.3333 50.0062 19.3333H34.6771C21.3302 19.3333 10.5104 30.1532 10.5104 43.5C10.5104 56.8468 21.3302 67.6667 34.6771 67.6667H50.0062C52.5701 67.6667 55.0288 66.6483 56.8418 64.8353L60.8457 60.8314C62.6587 59.0184 65.1174 58 67.6813 58H83.0104C96.3572 58 107.177 47.1801 107.177 33.8333C107.177 20.4866 96.3572 9.66667 83.0104 9.66667H67.6813Z" fill="black"/>
            </svg>
            <h3 class="text-xl font-medium">16commerce</h3>
          </div>
          <p class="text-gray-500 text-lg">P2P Resale Marketplaces</p>
        </div>

        <div>
          <ul class="space-y-4 text-sm font-medium">
            <li><a href="#contact" class="hover:underline">Get in touch</a></li>
            <li><a href="#platform" class="hover:underline">Platform</a></li>
            <li><a href="#benefits" class="hover:underline">Benefits</a></li>
          </ul>
        </div>

        <div>
          <ul class="space-y-4 text-sm font-medium">
            <li><a href="https://linkedin.com" target="_blank" rel="noopener noreferrer" class="hover:underline">LinkedIn</a></li>
            <li><a href="https://twitter.com" target="_blank" rel="noopener noreferrer" class="hover:underline">X</a></li>
          </ul>
        </div>
      </div>

      <div class="flex flex-col md:flex-row justify-between items-end text-[10px] text-gray-400 uppercase tracking-wider gap-4">
        <div class="flex gap-8">
          <span>16commerce 2025</span>
          <span>Founded by Ummu Aisyah</span>
        </div>
        <div class="flex gap-8">
          <a href="#" class="hover:text-gray-600">Terms of use</a>
          <a href="#" class="hover:text-gray-600">Privacy Policy</a>
        </div>
      </div>
    </div>
  </footer>

  <!-- Cookie Banner -->
  {#if showCookieBanner}
    <div class="fixed bottom-6 right-6 max-w-sm bg-white border border-gray-100 shadow-xl p-6 rounded-sm z-50 text-xs text-gray-600">
      <p class="mb-4 leading-relaxed">
        We use cookies. See our <a href="#" class="underline text-black">Privacy Policy</a> for more information.
      </p>
      <button onclick={() => showCookieBanner = false} class="bg-black text-white px-4 py-2 rounded-sm font-medium hover:bg-gray-800 transition-colors">
        Got it
      </button>
    </div>
  {/if}
</div>

<style>
  :global(body) {
    font-family: 'Inter', sans-serif;
  }
  .perspective-1000 {
    perspective: 1000px;
  }
  .transform-style-3d {
    transform-style: preserve-3d;
  }
</style>


<script lang="ts">
  import Navbar from '$lib/Navbar.svelte';
  import Footer from '$lib/Footer.svelte';
  import Button from '$lib/Button.svelte';
</script>

<div class="min-h-screen font-sans text-dark bg-cream overflow-x-hidden">
  <Navbar />

  <!-- Hero Section -->
  <section class="pt-32 pb-16 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto text-center">
    <div class="mb-6">
      <span class="text-xs font-bold tracking-widest text-gray-500 uppercase">Crowdfunded Collectible Plush</span>
    </div>
    <h1 class="text-5xl md:text-7xl font-serif mb-6 leading-tight">
      Character-driven comfort <br class="hidden md:block" /> fans actually want
    </h1>
    <p class="text-lg md:text-xl text-gray-600 max-w-2xl mx-auto mb-10 leading-relaxed">
      Limited-edition plush collectibles inspired by your favorite characters. 
      Co-created with creators, backed by fans, delivered with love.
    </p>
    <div class="flex flex-col sm:flex-row items-center justify-center gap-4 mb-20">
      <Button href="#" type="primary">Back a Plush &rarr;</Button>
      <Button href="#" type="outline">View Collection</Button>
    </div>

    <!-- Hero Image Placeholder -->
    <div class="relative w-full max-w-5xl mx-auto rounded-2xl overflow-hidden shadow-2xl border border-gray-200 bg-gradient-to-br from-pink-50 to-purple-50 aspect-[16/9] mb-16 group">
      <!-- Plush Display -->
      <div class="absolute inset-0 flex items-center justify-center p-8">
        <div class="grid grid-cols-3 gap-6 w-full max-w-4xl">
            <!-- Plush 1 -->
            <div class="bg-white rounded-2xl p-6 shadow-lg transform hover:scale-105 transition-transform">
                <div class="aspect-square bg-gradient-to-br from-pink-200 to-pink-300 rounded-xl mb-4 flex items-center justify-center">
                    <svg viewBox="0 0 100 100" class="w-20 h-20" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <circle cx="50" cy="50" r="35" fill="oklch(0.592 0.249 0.584)"/>
                        <circle cx="40" cy="45" r="4" fill="white"/>
                        <circle cx="60" cy="45" r="4" fill="white"/>
                        <path d="M40 60 Q50 65 60 60" stroke="white" stroke-width="2" stroke-linecap="round"/>
                    </svg>
                </div>
                <div class="text-center">
                    <div class="h-3 w-24 bg-gray-200 rounded mx-auto mb-2"></div>
                    <div class="h-2 w-16 bg-gray-100 rounded mx-auto"></div>
                </div>
            </div>
            
            <!-- Plush 2 (Featured) -->
            <div class="bg-white rounded-2xl p-8 shadow-xl transform scale-110 z-10">
                <div class="aspect-square bg-gradient-to-br from-purple-200 to-blue-200 rounded-xl mb-4 flex items-center justify-center relative">
                    <svg viewBox="0 0 100 100" class="w-24 h-24" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <ellipse cx="50" cy="55" rx="38" ry="35" fill="oklch(0.718 0.202 349.761)"/>
                        <circle cx="40" cy="50" r="5" fill="white"/>
                        <circle cx="60" cy="50" r="5" fill="white"/>
                        <path d="M38 65 Q50 72 62 65" stroke="white" stroke-width="3" stroke-linecap="round"/>
                        <ellipse cx="35" cy="45" rx="8" ry="10" fill="oklch(0.718 0.202 349.761)" opacity="0.3"/>
                        <ellipse cx="65" cy="45" rx="8" ry="10" fill="oklch(0.718 0.202 349.761)" opacity="0.3"/>
                    </svg>
                    <div class="absolute -top-2 -right-2 bg-primary-brand text-white text-xs px-2 py-1 rounded-full font-bold">NEW</div>
                </div>
                <div class="text-center">
                    <div class="h-3 w-28 bg-gray-200 rounded mx-auto mb-2"></div>
                    <div class="h-2 w-20 bg-primary-brand/30 rounded mx-auto"></div>
                </div>
            </div>
            
            <!-- Plush 3 -->
            <div class="bg-white rounded-2xl p-6 shadow-lg transform hover:scale-105 transition-transform">
                <div class="aspect-square bg-gradient-to-br from-yellow-200 to-orange-200 rounded-xl mb-4 flex items-center justify-center">
                    <svg viewBox="0 0 100 100" class="w-20 h-20" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M50 80C70 80 80 65 80 50C80 35 70 20 50 20C30 20 20 35 20 50C20 65 30 80 50 80Z" fill="oklch(0.656 0.241 354.308)"/>
                        <circle cx="38" cy="45" r="4" fill="white"/>
                        <circle cx="62" cy="45" r="4" fill="white"/>
                        <path d="M38 58 Q50 63 62 58" stroke="white" stroke-width="2" stroke-linecap="round"/>
                    </svg>
                </div>
                <div class="text-center">
                    <div class="h-3 w-24 bg-gray-200 rounded mx-auto mb-2"></div>
                    <div class="h-2 w-16 bg-gray-100 rounded mx-auto"></div>
                </div>
            </div>
        </div>
      </div>
      
      <!-- Decorative Elements -->
      <div class="absolute -left-12 bottom-12 w-24 h-24 bg-primary-brand rounded-full blur-2xl opacity-20"></div>
      <div class="absolute -right-12 top-12 w-32 h-32 bg-purple-400 rounded-full blur-2xl opacity-20"></div>
    </div>

    <!-- Social Proof -->
    <div class="text-center">
      <p class="text-sm text-gray-500 mb-6">Trusted by fans and creators worldwide</p>
      <div class="flex flex-wrap justify-center items-center gap-8 md:gap-12">
        <div class="flex items-center gap-2 text-gray-600">
          <svg class="w-5 h-5 text-primary-brand" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
          <span class="font-semibold">4.9/5</span>
          <span class="text-sm">from 2,400+ backers</span>
        </div>
        <div class="h-8 w-px bg-gray-300"></div>
        <div class="text-gray-600">
          <span class="font-bold text-2xl text-dark">12K+</span>
          <span class="text-sm ml-2">Community Members</span>
        </div>
        <div class="h-8 w-px bg-gray-300"></div>
        <div class="text-gray-600">
          <span class="font-bold text-2xl text-dark">25+</span>
          <span class="text-sm ml-2">Successful Campaigns</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Stats Section -->
  <section class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16 max-w-3xl mx-auto">
        From fan-favorite characters to collectible comfort
      </h2>
      
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-16">
        <div class="bg-gray-50 p-8 rounded-2xl text-center">
          <div class="text-4xl font-serif font-medium mb-2">First-Edition</div>
          <div class="text-xs font-bold text-gray-400 tracking-widest uppercase">Limited Collectibles</div>
        </div>
        <div class="bg-gray-50 p-8 rounded-2xl text-center">
          <div class="text-4xl font-serif font-medium mb-2">Co-Created</div>
          <div class="text-xs font-bold text-gray-400 tracking-widest uppercase">With Creators</div>
        </div>
        <div class="bg-gray-50 p-8 rounded-2xl text-center">
          <div class="text-4xl font-serif font-medium mb-2">Fan-Backed</div>
          <div class="text-xs font-bold text-gray-400 tracking-widest uppercase">Crowdfunded Drops</div>
        </div>
      </div>

      <!-- Plush Collection Carousel -->
      <div class="flex gap-4 overflow-hidden relative">
        <div class="absolute inset-y-0 left-0 w-20 bg-gradient-to-r from-white to-transparent z-10"></div>
        <div class="absolute inset-y-0 right-0 w-20 bg-gradient-to-l from-white to-transparent z-10"></div>
        
        <div class="flex gap-4 animate-scroll">
            <!-- Plush 1 -->
            <div class="w-64 h-80 bg-gradient-to-br from-pink-100 to-pink-200 rounded-2xl flex-shrink-0 relative overflow-hidden group flex items-center justify-center">
                <svg viewBox="0 0 100 100" class="w-32 h-32" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="50" cy="50" r="35" fill="oklch(0.592 0.249 0.584)"/>
                    <circle cx="40" cy="45" r="5" fill="white"/>
                    <circle cx="60" cy="45" r="5" fill="white"/>
                    <path d="M40 60 Q50 65 60 60" stroke="white" stroke-width="3" stroke-linecap="round"/>
                </svg>
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-2 py-1 rounded-full text-xs font-bold">
                    Limited Edition
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/60 to-transparent p-4 text-white">
                    <div class="font-bold">Cozy Companion</div>
                    <div class="text-xs opacity-80">Series 1</div>
                </div>
            </div>
            <!-- Plush 2 -->
            <div class="w-64 h-80 bg-gradient-to-br from-purple-100 to-blue-200 rounded-2xl flex-shrink-0 relative overflow-hidden group flex items-center justify-center">
                <svg viewBox="0 0 100 100" class="w-32 h-32" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <ellipse cx="50" cy="55" rx="38" ry="35" fill="oklch(0.718 0.202 349.761)"/>
                    <circle cx="40" cy="50" r="5" fill="white"/>
                    <circle cx="60" cy="50" r="5" fill="white"/>
                    <path d="M38 65 Q50 72 62 65" stroke="white" stroke-width="3" stroke-linecap="round"/>
                </svg>
                <div class="absolute top-4 left-4 bg-primary-brand text-white px-2 py-1 rounded-full text-xs font-bold">
                    Funding Now
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/60 to-transparent p-4 text-white">
                    <div class="font-bold">Dream Friend</div>
                    <div class="text-xs opacity-80">Series 2</div>
                </div>
            </div>
            <!-- Plush 3 -->
            <div class="w-64 h-80 bg-gradient-to-br from-yellow-100 to-orange-200 rounded-2xl flex-shrink-0 relative overflow-hidden group flex items-center justify-center">
                <svg viewBox="0 0 100 100" class="w-32 h-32" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M50 80C70 80 80 65 80 50C80 35 70 20 50 20C30 20 20 35 20 50C20 65 30 80 50 80Z" fill="oklch(0.656 0.241 354.308)"/>
                    <circle cx="38" cy="45" r="5" fill="white"/>
                    <circle cx="62" cy="45" r="5" fill="white"/>
                    <path d="M38 58 Q50 63 62 58" stroke="white" stroke-width="3" stroke-linecap="round"/>
                </svg>
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-2 py-1 rounded-full text-xs font-bold">
                    Coming Soon
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/60 to-transparent p-4 text-white">
                    <div class="font-bold">Sunshine Pal</div>
                    <div class="text-xs opacity-80">Series 3</div>
                </div>
            </div>
             <!-- Plush 4 -->
            <div class="w-64 h-80 bg-gradient-to-br from-blue-100 to-cyan-200 rounded-2xl flex-shrink-0 relative overflow-hidden group flex items-center justify-center">
                <svg viewBox="0 0 100 100" class="w-32 h-32" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <ellipse cx="50" cy="52" rx="36" ry="38" fill="oklch(0.525 0.223 3.958)"/>
                    <circle cx="42" cy="48" r="4" fill="white"/>
                    <circle cx="58" cy="48" r="4" fill="white"/>
                    <path d="M42 62 Q50 68 58 62" stroke="white" stroke-width="2" stroke-linecap="round"/>
                </svg>
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-2 py-1 rounded-full text-xs font-bold">
                    Limited Edition
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/60 to-transparent p-4 text-white">
                    <div class="font-bold">Ocean Buddy</div>
                    <div class="text-xs opacity-80">Series 1</div>
                </div>
            </div>
             <!-- Plush 5 -->
            <div class="w-64 h-80 bg-gradient-to-br from-green-100 to-emerald-200 rounded-2xl flex-shrink-0 relative overflow-hidden group flex items-center justify-center">
                <svg viewBox="0 0 100 100" class="w-32 h-32" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="50" cy="50" r="34" fill="oklch(0.459 0.187 3.815)"/>
                    <circle cx="41" cy="46" r="4" fill="white"/>
                    <circle cx="59" cy="46" r="4" fill="white"/>
                    <path d="M41 60 Q50 66 59 60" stroke="white" stroke-width="2" stroke-linecap="round"/>
                </svg>
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-2 py-1 rounded-full text-xs font-bold">
                    Sold Out
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-black/60 to-transparent p-4 text-white">
                    <div class="font-bold">Forest Friend</div>
                    <div class="text-xs opacity-80">Series 1</div>
                </div>
            </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Problem/Solution Section -->
  <section class="bg-dark text-white py-24 overflow-hidden">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-4">Fan merch deserves <br /> better than this</h2>
      <p class="text-center text-gray-400 mb-16">Generic products don't capture the magic fans feel for their favorite characters.</p>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
        <!-- The Problem -->
        <div>
          <h3 class="text-xl font-serif mb-2">Generic Merch</h3>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            Low-effort creator products flood the market. Mass-produced, soulless items that don't reflect the care fans have for characters they love.
          </p>
          <div class="bg-gray-800/50 rounded-xl p-6 border border-gray-700 relative">
             <div class="space-y-3">
                <div class="flex items-center gap-3 opacity-50">
                    <div class="w-12 h-12 bg-gray-700 rounded"></div>
                    <div class="flex-1">
                        <div class="h-3 bg-gray-700 rounded mb-2"></div>
                        <div class="h-2 bg-gray-700 rounded w-2/3"></div>
                    </div>
                </div>
                <div class="flex items-center gap-3 opacity-50">
                    <div class="w-12 h-12 bg-gray-700 rounded"></div>
                    <div class="flex-1">
                        <div class="h-3 bg-gray-700 rounded mb-2"></div>
                        <div class="h-2 bg-gray-700 rounded w-2/3"></div>
                    </div>
                </div>
                <div class="flex items-center gap-3 opacity-50">
                    <div class="w-12 h-12 bg-gray-700 rounded"></div>
                    <div class="flex-1">
                        <div class="h-3 bg-gray-700 rounded mb-2"></div>
                        <div class="h-2 bg-gray-700 rounded w-2/3"></div>
                    </div>
                </div>
             </div>
             <div class="absolute top-4 right-4 text-xs font-bold text-red-400">❌ Mass-produced</div>
          </div>
        </div>

        <!-- The Solution -->
        <div>
          <h3 class="text-xl font-serif mb-2">Glimkin Collectibles</h3>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            Limited-edition, co-created plush that capture character essence. Each drop is validated by community demand before production.
          </p>
          <div class="relative h-64 flex items-center justify-center">
             <!-- Central Plush -->
             <div class="relative z-10 w-32 h-32 bg-gradient-to-br from-primary-brand to-primary-light rounded-full flex items-center justify-center shadow-2xl">
                <svg viewBox="0 0 100 100" class="w-20 h-20" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="50" cy="50" r="35" fill="white"/>
                    <circle cx="40" cy="45" r="5" fill="oklch(0.592 0.249 0.584)"/>
                    <circle cx="60" cy="45" r="5" fill="oklch(0.592 0.249 0.584)"/>
                    <path d="M40 60 Q50 65 60 60" stroke="oklch(0.592 0.249 0.584)" stroke-width="3" stroke-linecap="round"/>
                </svg>
             </div>
             <!-- Floating Elements -->
             <div class="absolute top-8 left-8 bg-primary-brand/20 backdrop-blur px-3 py-1.5 rounded-full text-xs font-bold border border-primary-brand/30">
                ✨ Co-created
             </div>
             <div class="absolute bottom-8 right-8 bg-primary-brand/20 backdrop-blur px-3 py-1.5 rounded-full text-xs font-bold border border-primary-brand/30">
                🎯 Limited
             </div>
             <div class="absolute bottom-12 left-12 bg-primary-brand/20 backdrop-blur px-3 py-1.5 rounded-full text-xs font-bold border border-primary-brand/30">
                💝 Fan-backed
             </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Features Section 1 -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16 max-w-2xl mx-auto">
        How Glimkin brings characters to life
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- Card 1: Co-Creation -->
        <div class="lg:col-span-2 bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden relative group">
            <div class="mb-8">
                <h3 class="text-xl font-serif mb-2">Co-created with creators</h3>
                <p class="text-gray-500 text-sm">We partner with content creators to bring their beloved characters to life as premium plush collectibles.</p>
            </div>
            <div class="bg-pink-50 rounded-xl p-6 h-64 relative border border-pink-100 flex items-center justify-center">
                <div class="flex items-center gap-8">
                    <div class="text-center">
                        <div class="w-20 h-20 bg-gradient-to-br from-primary-brand to-primary-light rounded-full mb-3 flex items-center justify-center">
                            <span class="text-2xl">🎨</span>
                        </div>
                        <div class="text-xs font-bold text-gray-600">Creator</div>
                    </div>
                    <div class="text-3xl text-primary-brand">+</div>
                    <div class="text-center">
                        <div class="w-20 h-20 bg-gradient-to-br from-purple-400 to-pink-400 rounded-full mb-3 flex items-center justify-center">
                            <span class="text-2xl">🧸</span>
                        </div>
                        <div class="text-xs font-bold text-gray-600">Glimkin</div>
                    </div>
                    <div class="text-3xl text-primary-brand">=</div>
                    <div class="text-center">
                        <div class="w-24 h-24 bg-gradient-to-br from-pink-200 to-purple-200 rounded-2xl mb-3 flex items-center justify-center shadow-lg">
                            <svg viewBox="0 0 100 100" class="w-16 h-16" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <circle cx="50" cy="50" r="30" fill="oklch(0.592 0.249 0.584)"/>
                                <circle cx="42" cy="45" r="4" fill="white"/>
                                <circle cx="58" cy="45" r="4" fill="white"/>
                                <path d="M42 58 Q50 63 58 58" stroke="white" stroke-width="2" stroke-linecap="round"/>
                            </svg>
                        </div>
                        <div class="text-xs font-bold text-primary-brand">Magic ✨</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Card 2: Crowdfunded -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
            <div class="mb-8">
                <h3 class="text-xl font-serif mb-2">Community-validated demand</h3>
                <p class="text-gray-500 text-sm">Every plush is crowdfunded first. We only produce what fans actually want.</p>
            </div>
            <div class="bg-pink-50 rounded-xl h-48 relative overflow-hidden flex items-center justify-center">
                <div class="text-center">
                    <div class="text-5xl font-serif font-bold text-primary-brand mb-2">250%</div>
                    <div class="text-sm text-gray-600 mb-4">Avg. funding goal reached</div>
                    <div class="flex gap-1 justify-center">
                        {#each Array(10) as _}
                            <div class="w-2 h-12 bg-primary-brand/80 rounded-full"></div>
                        {/each}
                    </div>
                </div>
            </div>
        </div>

        <!-- Card 3: Premium Quality -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
             <div class="h-48 bg-pink-50 rounded-xl mb-6 p-4 relative flex items-center justify-center">
                <div class="relative">
                    <div class="w-32 h-32 bg-gradient-to-br from-primary-brand to-primary-light rounded-2xl shadow-xl flex items-center justify-center transform rotate-[-5deg]">
                        <svg viewBox="0 0 100 100" class="w-20 h-20" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <circle cx="50" cy="50" r="30" fill="white"/>
                            <circle cx="42" cy="45" r="4" fill="oklch(0.592 0.249 0.584)"/>
                            <circle cx="58" cy="45" r="4" fill="oklch(0.592 0.249 0.584)"/>
                            <path d="M42 58 Q50 63 58 58" stroke="oklch(0.592 0.249 0.584)" stroke-width="2" stroke-linecap="round"/>
                        </svg>
                    </div>
                    <div class="absolute -top-2 -right-2 bg-yellow-400 text-yellow-900 px-2 py-1 rounded-full text-xs font-bold">★ Premium</div>
                </div>
             </div>
             <h3 class="text-xl font-serif mb-2">Premium materials</h3>
             <p class="text-gray-500 text-sm">Soft, huggable, and built to last. Each plush is crafted with care and attention to detail.</p>
        </div>

        <!-- Card 4: Limited Editions -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
             <div class="h-48 bg-pink-50 rounded-xl mb-6 p-4 flex items-center justify-center">
                <div class="text-center space-y-3">
                    <div class="inline-block bg-primary-brand text-white px-4 py-2 rounded-full text-sm font-bold">
                        #247 / 500
                    </div>
                    <div class="text-xs text-gray-500">Each plush is numbered</div>
                    <div class="flex gap-2 justify-center">
                        <div class="w-3 h-3 bg-primary-brand rounded-full"></div>
                        <div class="w-3 h-3 bg-primary-brand rounded-full"></div>
                        <div class="w-3 h-3 bg-primary-brand rounded-full"></div>
                        <div class="w-3 h-3 bg-gray-200 rounded-full"></div>
                        <div class="w-3 h-3 bg-gray-200 rounded-full"></div>
                    </div>
                </div>
             </div>
             <h3 class="text-xl font-serif mb-2">First-edition collectibles</h3>
             <p class="text-gray-500 text-sm">Limited runs mean your plush is truly special. Each one is numbered and authenticated.</p>
        </div>

        <!-- Card 5: Community -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
             <div class="h-48 bg-pink-50 rounded-xl mb-6 p-4 flex items-center justify-center relative">
                 <div class="grid grid-cols-3 gap-2">
                    {#each Array(9) as _, i}
                        <div class="w-12 h-12 rounded-full bg-gradient-to-br from-primary-brand to-primary-light flex items-center justify-center text-white text-xs font-bold opacity-{100 - i * 10}">
                            {i === 0 ? '😊' : i === 1 ? '🎉' : i === 2 ? '💕' : i === 3 ? '✨' : i === 4 ? '🌟' : i === 5 ? '🎨' : i === 6 ? '🧸' : i === 7 ? '💖' : '🎁'}
                        </div>
                    {/each}
                 </div>
             </div>
             <h3 class="text-xl font-serif mb-2">Join the community</h3>
             <p class="text-gray-500 text-sm">Connect with fellow collectors, share photos, and vote on future designs in our Discord.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonial 1 -->
  <section class="py-16 bg-cream">
    <div class="max-w-4xl mx-auto px-4 text-center">
        <div class="flex justify-center mb-8">
            <div class="flex gap-1">
                {#each Array(5) as _}
                    <svg class="w-6 h-6 text-primary-brand" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"/></svg>
                {/each}
            </div>
        </div>
        <blockquote class="text-2xl md:text-3xl font-serif leading-relaxed mb-8">
            "I've been collecting plush for years, but Glimkin is different. The quality is incredible, and knowing it's a limited edition makes it so much more special. My Dream Friend sits on my desk every day!"
        </blockquote>
        <div class="flex items-center justify-center gap-4">
            <div class="w-12 h-12 rounded-full bg-gradient-to-br from-primary-brand to-primary-light"></div>
            <div class="text-left">
                <div class="font-bold text-sm">Sarah Chen</div>
                <div class="text-xs text-gray-500">Collector & Community Member</div>
            </div>
        </div>
    </div>
  </section>

  <!-- Features Section 2 -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16">
        How crowdfunding <br /> brings plush to life
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- Card 1 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-pink-50 rounded-xl h-64 mb-8 p-4 relative overflow-hidden flex items-center justify-center">
                <div class="text-center">
                    <div class="text-6xl mb-4">🎯</div>
                    <div class="text-2xl font-serif font-bold mb-2">Step 1</div>
                    <div class="text-sm text-gray-600">Campaign Launch</div>
                </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Discover & back</h3>
            <p class="text-gray-500 text-sm">Browse active campaigns and back the plush you love. Every backer helps bring the character to life.</p>
        </div>

        <!-- Card 2 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-pink-50 rounded-xl h-64 mb-8 p-4 flex items-center justify-center">
                 <div class="relative w-full max-w-xs">
                    <div class="bg-white rounded-xl shadow-lg p-6">
                        <div class="flex justify-between items-center mb-4">
                            <div class="text-xs font-bold text-gray-400">FUNDING PROGRESS</div>
                            <div class="text-xs font-bold text-primary-brand">250%</div>
                        </div>
                        <div class="h-3 bg-gray-100 rounded-full overflow-hidden mb-2">
                            <div class="h-full bg-gradient-to-r from-primary-brand to-primary-light rounded-full" style="width: 100%"></div>
                        </div>
                        <div class="text-xs text-gray-500 text-center">$12,500 of $5,000 goal</div>
                    </div>
                 </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Community funding</h3>
            <p class="text-gray-500 text-sm">Watch the campaign grow as fans rally together. Hit the goal and production begins!</p>
        </div>

        <!-- Card 3 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-pink-50 rounded-xl h-64 mb-8 p-4 flex items-center justify-center">
                <div class="text-center space-y-4">
                    <div class="inline-flex items-center gap-3 bg-white px-6 py-3 rounded-full shadow-lg">
                        <div class="w-3 h-3 bg-yellow-400 rounded-full animate-pulse"></div>
                        <span class="text-sm font-bold">In Production</span>
                    </div>
                    <div class="flex justify-center gap-2">
                        <div class="w-2 h-2 bg-primary-brand rounded-full animate-bounce"></div>
                        <div class="w-2 h-2 bg-primary-brand rounded-full animate-bounce" style="animation-delay: 0.1s"></div>
                        <div class="w-2 h-2 bg-primary-brand rounded-full animate-bounce" style="animation-delay: 0.2s"></div>
                    </div>
                </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Premium production</h3>
            <p class="text-gray-500 text-sm">Once funded, we craft each plush with premium materials and attention to detail.</p>
        </div>

        <!-- Card 4 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-pink-50 rounded-xl h-64 mb-8 p-4 flex items-center justify-center">
                <div class="relative">
                    <div class="w-40 h-40 bg-gradient-to-br from-primary-brand to-primary-light rounded-2xl shadow-2xl flex items-center justify-center transform rotate-[-5deg]">
                        <svg viewBox="0 0 100 100" class="w-24 h-24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <circle cx="50" cy="50" r="35" fill="white"/>
                            <circle cx="40" cy="45" r="5" fill="oklch(0.592 0.249 0.584)"/>
                            <circle cx="60" cy="45" r="5" fill="oklch(0.592 0.249 0.584)"/>
                            <path d="M40 60 Q50 65 60 60" stroke="oklch(0.592 0.249 0.584)" stroke-width="3" stroke-linecap="round"/>
                        </svg>
                    </div>
                    <div class="absolute -top-3 -right-3 bg-white p-2 rounded-full shadow-lg text-2xl">📦</div>
                </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Delivered to your door</h3>
            <p class="text-gray-500 text-sm">Your first-edition collectible arrives ready to display, hug, or gift. Each one is numbered and special.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Join Community CTA -->
  <section class="py-24 bg-cream relative overflow-hidden">
    <!-- Floating Plush Background -->
    <div class="absolute inset-0 opacity-10 pointer-events-none">
        <div class="absolute top-10 left-10 w-16 h-16 bg-primary-brand rounded-full transform rotate-12"></div>
        <div class="absolute top-20 right-20 w-12 h-12 bg-primary-light rounded-full transform -rotate-6"></div>
        <div class="absolute bottom-20 left-1/3 w-14 h-14 bg-primary-brand rounded-full transform rotate-45"></div>
        <div class="absolute bottom-10 right-1/4 w-10 h-10 bg-primary-light rounded-full transform -rotate-12"></div>
    </div>

    <div class="max-w-4xl mx-auto px-4 text-center relative z-10">
        <div class="inline-block bg-primary-brand/10 text-primary-brand px-4 py-1 rounded-full text-xs font-bold mb-6">
            Join the Glimkin Community →
        </div>
        <h2 class="text-4xl md:text-6xl font-serif mb-4">25+ successful campaigns <br /> and counting</h2>
        <p class="text-gray-500 mb-10">Over 12,000 collectors worldwide trust Glimkin</p>
        
        <div class="flex justify-center gap-4">
            <Button href="#" type="primary">Back a Plush &rarr;</Button>
            <Button href="#" type="white">Browse Collection</Button>
        </div>
    </div>
  </section>

  <!-- Why Fans Love Glimkin -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16">
        Why fans choose <br /> Glimkin collectibles
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- Left Large Card -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 md:row-span-2 flex flex-col">
            <div class="mb-8">
                <h3 class="text-xl font-serif mb-2">Authentic character love</h3>
                <p class="text-gray-500 text-sm">Not just merch - each plush captures the essence of characters fans genuinely care about. Co-created with the original creators.</p>
            </div>
            <div class="flex-1 bg-pink-50 rounded-2xl relative overflow-hidden min-h-[300px] flex items-center justify-center">
                <div class="absolute inset-0 bg-[radial-gradient(circle_at_center,_var(--tw-gradient-stops))] from-primary-brand/20 to-transparent"></div>
                <!-- Central Plush -->
                <div class="relative z-10">
                    <div class="w-48 h-48 bg-gradient-to-br from-primary-brand to-primary-light rounded-3xl shadow-2xl flex items-center justify-center transform hover:scale-105 transition-transform">
                        <svg viewBox="0 0 100 100" class="w-32 h-32" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <circle cx="50" cy="50" r="35" fill="white"/>
                            <circle cx="40" cy="45" r="6" fill="oklch(0.592 0.249 0.584)"/>
                            <circle cx="60" cy="45" r="6" fill="oklch(0.592 0.249 0.584)"/>
                            <path d="M38 60 Q50 68 62 60" stroke="oklch(0.592 0.249 0.584)" stroke-width="3" stroke-linecap="round"/>
                            <ellipse cx="35" cy="42" rx="10" ry="12" fill="oklch(0.592 0.249 0.584)" opacity="0.2"/>
                            <ellipse cx="65" cy="42" rx="10" ry="12" fill="oklch(0.592 0.249 0.584)" opacity="0.2"/>
                        </svg>
                    </div>
                    <div class="absolute -top-4 -right-4 bg-yellow-400 text-yellow-900 px-3 py-1.5 rounded-full text-xs font-bold shadow-lg">
                        ✨ Authentic
                    </div>
                </div>
            </div>
        </div>

        <!-- Right Top Card -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="flex justify-between items-start mb-4">
                <div>
                     <h3 class="text-xl font-serif mb-2">True collectible value</h3>
                     <p class="text-gray-500 text-sm">Limited first-editions with numbered certificates. Each plush is a genuine collectible that holds its value.</p>
                </div>
                <span class="bg-primary-brand/10 text-primary-brand px-2 py-1 rounded text-xs font-bold">Limited</span>
            </div>
            <div class="bg-pink-50 rounded-xl h-40 flex items-center justify-center">
                <div class="text-center">
                    <div class="text-5xl font-serif font-bold text-primary-brand mb-2">#127</div>
                    <div class="text-sm text-gray-600 mb-1">of 500</div>
                    <div class="inline-block bg-white px-4 py-2 rounded-full shadow-sm text-xs font-bold">
                        Certificate of Authenticity
                    </div>
                </div>
            </div>
        </div>

        <!-- Right Bottom Card (Testimonial) -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 flex gap-6 items-center">
            <div class="w-24 h-24 bg-gradient-to-br from-primary-brand to-primary-light rounded-full flex-shrink-0 overflow-hidden flex items-center justify-center text-white text-3xl">
                😊
            </div>
            <div>
                <div class="text-primary-brand text-4xl font-serif leading-none mb-2">"</div>
                <p class="text-sm text-gray-600 italic mb-4">Finally, merch that actually captures the characters I love. The quality is amazing and it feels special to own #342 of 500.</p>
                <div class="text-xs font-bold">Alex Rivera</div>
                <div class="text-[10px] text-gray-400">Early Backer & Collector</div>
            </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Community Gallery -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16 max-w-2xl mx-auto">
        Join thousands of collectors worldwide
      </h2>

      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-4">
         <!-- Row 1 -->
         <div class="aspect-square bg-gradient-to-br from-pink-200 to-pink-300 rounded-2xl relative overflow-hidden group flex items-center justify-center">
            <svg viewBox="0 0 100 100" class="w-20 h-20" fill="none" xmlns="http://www.w3.org/2000/svg">
                <circle cx="50" cy="50" r="30" fill="oklch(0.592 0.249 0.584)"/>
                <circle cx="42" cy="45" r="4" fill="white"/>
                <circle cx="58" cy="45" r="4" fill="white"/>
                <path d="M42 58 Q50 63 58 58" stroke="white" stroke-width="2" stroke-linecap="round"/>
            </svg>
            <div class="absolute bottom-4 left-4 text-white font-bold text-xs">Cozy Companion</div>
         </div>
         <div class="aspect-square bg-white rounded-2xl flex items-center justify-center border border-gray-100">
            <div class="text-center">
                <div class="text-4xl mb-2">⭐</div>
                <div class="text-sm font-bold">4.9/5</div>
                <div class="text-xs text-gray-500">Rating</div>
            </div>
         </div>
         <div class="col-span-2 bg-[#FFF9C4] rounded-2xl p-8 flex flex-col justify-between">
            <div class="text-4xl font-serif text-yellow-600">"</div>
            <p class="text-lg font-serif leading-relaxed">I've backed 5 Glimkin campaigns and every single one exceeded my expectations. The quality is unmatched!</p>
            <div class="flex justify-between items-end">
                <div class="text-xs">
                    <div class="font-bold">Jamie Lee</div>
                    <div class="text-gray-500">Collector since 2023</div>
                </div>
                <div class="text-xl">💕</div>
            </div>
         </div>

         <!-- Row 2 -->
         <div class="col-span-2 bg-gradient-to-br from-purple-200 to-blue-200 rounded-2xl flex items-center justify-center p-8">
            <svg viewBox="0 0 100 100" class="w-32 h-32" fill="none" xmlns="http://www.w3.org/2000/svg">
                <ellipse cx="50" cy="55" rx="35" ry="32" fill="oklch(0.718 0.202 349.761)"/>
                <circle cx="40" cy="50" r="5" fill="white"/>
                <circle cx="60" cy="50" r="5" fill="white"/>
                <path d="M38 65 Q50 72 62 65" stroke="white" stroke-width="3" stroke-linecap="round"/>
            </svg>
         </div>
         <div class="aspect-square bg-gradient-to-br from-yellow-200 to-orange-200 rounded-2xl relative overflow-hidden group flex items-center justify-center">
             <svg viewBox="0 0 100 100" class="w-20 h-20" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M50 80C70 80 80 65 80 50C80 35 70 20 50 20C30 20 20 35 20 50C20 65 30 80 50 80Z" fill="oklch(0.656 0.241 354.308)"/>
                <circle cx="38" cy="45" r="4" fill="white"/>
                <circle cx="62" cy="45" r="4" fill="white"/>
                <path d="M38 58 Q50 63 62 58" stroke="white" stroke-width="2" stroke-linecap="round"/>
            </svg>
             <div class="absolute bottom-4 left-4 text-white font-bold text-xs">Sunshine Pal</div>
         </div>
         <div class="aspect-square bg-white rounded-2xl relative overflow-hidden group flex items-center justify-center border border-gray-100">
             <div class="text-center">
                <div class="text-3xl font-serif font-bold text-primary-brand">12K+</div>
                <div class="text-xs text-gray-500">Community</div>
             </div>
         </div>

         <!-- Row 3 -->
         <div class="col-span-2 bg-[#FFE6F0] rounded-2xl p-8 flex flex-col justify-between">
            <div class="text-4xl font-serif text-primary-brand">"</div>
            <p class="text-lg font-serif leading-relaxed">My Dream Friend plush sits on my desk and makes me smile every day. Worth every penny!</p>
            <div class="flex justify-between items-end">
                <div class="text-xs">
                    <div class="font-bold">Taylor Kim</div>
                    <div class="text-gray-500">Proud Owner</div>
                </div>
                <div class="text-xl">✨</div>
            </div>
         </div>
         <div class="col-span-2 bg-gradient-to-br from-blue-200 to-cyan-200 rounded-2xl flex items-center justify-center p-8">
             <svg viewBox="0 0 100 100" class="w-32 h-32" fill="none" xmlns="http://www.w3.org/2000/svg">
                <ellipse cx="50" cy="52" rx="33" ry="35" fill="oklch(0.525 0.223 3.958)"/>
                <circle cx="42" cy="48" r="4" fill="white"/>
                <circle cx="58" cy="48" r="4" fill="white"/>
                <path d="M42 62 Q50 68 58 62" stroke="white" stroke-width="2" stroke-linecap="round"/>
            </svg>
         </div>
         
         <!-- Row 4 -->
         <div class="aspect-square bg-gradient-to-br from-green-200 to-emerald-200 rounded-2xl relative overflow-hidden group flex items-center justify-center">
             <svg viewBox="0 0 100 100" class="w-20 h-20" fill="none" xmlns="http://www.w3.org/2000/svg">
                <circle cx="50" cy="50" r="30" fill="oklch(0.459 0.187 3.815)"/>
                <circle cx="41" cy="46" r="4" fill="white"/>
                <circle cx="59" cy="46" r="4" fill="white"/>
                <path d="M41 60 Q50 66 59 60" stroke="white" stroke-width="2" stroke-linecap="round"/>
            </svg>
             <div class="absolute bottom-4 left-4 text-white font-bold text-xs">Forest Friend</div>
         </div>
         <div class="aspect-square bg-white rounded-2xl relative overflow-hidden group flex items-center justify-center border border-gray-100">
             <div class="text-center">
                <div class="text-3xl font-serif font-bold text-primary-brand">25+</div>
                <div class="text-xs text-gray-500">Campaigns</div>
             </div>
         </div>
         <div class="col-span-2 bg-white rounded-2xl flex items-center justify-center border border-gray-100 p-8">
             <div class="text-center">
                <div class="text-2xl font-bold mb-2">Limited. Loved. Collectible.</div>
                <div class="text-sm text-gray-500">Every Glimkin plush tells a story</div>
             </div>
         </div>
      </div>
    </div>
  </section>

  <!-- Primary CTA Section -->
  <section class="bg-primary-brand py-24 relative overflow-hidden">
    <div class="max-w-4xl mx-auto px-4 text-center relative z-10">
        <h2 class="text-4xl md:text-6xl font-serif mb-8 text-white">Start your collection <br /> with Glimkin today</h2>
        
        <div class="flex flex-col md:flex-row justify-center gap-6 mb-10 text-sm font-medium text-white/90">
            <div class="flex items-center gap-2">
                <div class="bg-white text-primary-brand rounded-full p-0.5"><svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg></div>
                First-edition collectibles
            </div>
            <div class="flex items-center gap-2">
                <div class="bg-white text-primary-brand rounded-full p-0.5"><svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg></div>
                Co-created with love
            </div>
        </div>

        <div class="flex justify-center gap-4">
            <Button href="#" type="primary">Back a Plush &rarr;</Button>
            <Button href="#" type="white">Browse Collection</Button>
        </div>
    </div>

    <!-- Bottom Illustration (Plush Pattern) -->
    <div class="absolute bottom-0 left-0 right-0 h-32 opacity-10 pointer-events-none flex items-end justify-center overflow-hidden">
        <svg width="1200" height="100" viewBox="0 0 1200 100" fill="none" xmlns="http://www.w3.org/2000/svg">
            {#each Array(12) as _, i}
                <circle cx="{100 * i + 50}" cy="50" r="30" fill="white" opacity="0.3"/>
                <circle cx="{100 * i + 40}" cy="45" r="4" fill="white"/>
                <circle cx="{100 * i + 60}" cy="45" r="4" fill="white"/>
            {/each}
        </svg>
    </div>
  </section>

  <!-- Featured Campaigns -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16">Featured Campaigns</h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <!-- Large Card Top -->
        <div class="md:col-span-2 bg-gradient-to-br from-pink-200 to-purple-200 rounded-3xl p-10 md:p-16 flex flex-col md:flex-row items-center gap-10">
            <div class="flex-1 flex items-center justify-center">
                <svg viewBox="0 0 100 100" class="w-48 h-48" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <ellipse cx="50" cy="55" rx="38" ry="35" fill="oklch(0.718 0.202 349.761)"/>
                    <circle cx="40" cy="50" r="5" fill="white"/>
                    <circle cx="60" cy="50" r="5" fill="white"/>
                    <path d="M38 65 Q50 72 62 65" stroke="white" stroke-width="3" stroke-linecap="round"/>
                    <ellipse cx="35" cy="45" rx="8" ry="10" fill="oklch(0.718 0.202 349.761)" opacity="0.3"/>
                    <ellipse cx="65" cy="45" rx="8" ry="10" fill="oklch(0.718 0.202 349.761)" opacity="0.3"/>
                </svg>
            </div>
            <div class="flex-1 bg-white/90 backdrop-blur rounded-2xl p-8 shadow-sm">
                <div class="text-xs font-bold text-primary-brand uppercase mb-4">Success Story</div>
                <h3 class="text-2xl font-serif mb-4">Dream Friend: 320% funded in 48 hours</h3>
                <p class="text-gray-500 text-sm mb-6">Co-created with popular artist @DreamyArt, this plush captured hearts and exceeded all expectations. Limited to 500 units, all sold out.</p>
                <div class="flex justify-between items-center">
                    <span class="text-xs text-gray-400">Featured Campaign</span>
                    <button class="bg-primary-brand text-white px-4 py-2 rounded-lg text-xs font-bold">View Campaign &rarr;</button>
                </div>
            </div>
        </div>

        <!-- Bottom Left -->
        <div class="bg-gradient-to-br from-yellow-200 to-orange-200 rounded-3xl p-8 flex flex-col justify-between h-96">
            <div class="flex items-center justify-center mb-8">
                <svg viewBox="0 0 100 100" class="w-32 h-32" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M50 80C70 80 80 65 80 50C80 35 70 20 50 20C30 20 20 35 20 50C20 65 30 80 50 80Z" fill="oklch(0.656 0.241 354.308)"/>
                    <circle cx="38" cy="45" r="5" fill="white"/>
                    <circle cx="62" cy="45" r="5" fill="white"/>
                    <path d="M38 58 Q50 63 62 58" stroke="white" stroke-width="3" stroke-linecap="round"/>
                </svg>
            </div>
            <div class="bg-white/90 backdrop-blur rounded-2xl p-6 shadow-sm mt-auto">
                <div class="text-xs font-bold text-primary-brand uppercase mb-2">Success Story</div>
                <h3 class="text-xl font-serif mb-4">Sunshine Pal: 1,200 backers strong</h3>
                <div class="flex justify-between items-center mt-4">
                    <span class="text-xs text-gray-400">Funding Now</span>
                    <button class="bg-primary-brand text-white px-3 py-1.5 rounded-lg text-xs font-bold">Back Now &rarr;</button>
                </div>
            </div>
        </div>

        <!-- Bottom Right -->
        <div class="bg-gradient-to-br from-blue-200 to-cyan-200 rounded-3xl p-8 flex flex-col justify-between h-96">
            <div class="flex items-center justify-center mb-8">
                <svg viewBox="0 0 100 100" class="w-32 h-32" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <ellipse cx="50" cy="52" rx="36" ry="38" fill="oklch(0.525 0.223 3.958)"/>
                    <circle cx="42" cy="48" r="4" fill="white"/>
                    <circle cx="58" cy="48" r="4" fill="white"/>
                    <path d="M42 62 Q50 68 58 62" stroke="white" stroke-width="2" stroke-linecap="round"/>
                </svg>
            </div>
            <div class="bg-white/90 backdrop-blur rounded-2xl p-6 shadow-sm mt-auto">
                <div class="text-xs font-bold text-primary-brand uppercase mb-2">Success Story</div>
                <h3 class="text-xl font-serif mb-4">Ocean Buddy: Sold out in 3 days</h3>
                <div class="flex justify-between items-center mt-4">
                    <span class="text-xs text-gray-400">Completed</span>
                    <button class="bg-gray-300 text-gray-600 px-3 py-1.5 rounded-lg text-xs font-bold">Sold Out</button>
                </div>
            </div>
        </div>
      </div>
    </div>
  </section>

  <!-- FAQ -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif mb-16">Frequently Asked Questions</h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-x-12 gap-y-6">
        {#each [
            "What is Glimkin?",
            "How does crowdfunding work?",
            "What makes Glimkin plush special?",
            "How long does shipping take?",
            "Are the plush really limited edition?",
            "Can I suggest a character?",
            "What if a campaign doesn't reach its goal?",
            "How do I join the community?"
        ] as question}
            <div class="border-b border-gray-200 py-4 flex justify-between items-center group cursor-pointer">
                <span class="font-medium text-lg group-hover:text-primary-brand transition-colors">{question}</span>
                <div class="w-6 h-6 rounded-full bg-dark text-white flex items-center justify-center text-sm group-hover:bg-primary-brand transition-colors">+</div>
            </div>
        {/each}
      </div>
    </div>
  </section>

  <Footer />
</div>

<style>
  /* Custom Scroll Animation */
  @keyframes scroll {
    0% { transform: translateX(0); }
    100% { transform: translateX(-50%); }
  }
  .animate-scroll {
    animation: scroll 20s linear infinite;
  }
  
  @keyframes spin-slow {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }
  .animate-spin-slow {
    animation: spin-slow 20s linear infinite;
  }
</style>


# paulkabonluxury
portfolio
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Paul Kabon Luxury Atelier | Handmade Leather Shoes, Bags & Accessories</title>
    <meta name="description" content="Discover bespoke handmade leather shoes, bags, belts, and custom accessories crafted with precision and purpose in Awka, Anambra State, Nigeria.">
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        onyx: '#0B0B0B',
                        charcoal: '#171717',
                        gold: {
                            DEFAULT: '#C5A059',
                            light: '#E5C178',
                            dark: '#9A7836'
                        },
                        ivory: '#F9F8F6',
                        tan: '#8B5A2B',
                        tanDark: '#5C3A18'
                    },
                    fontFamily: {
                        serif: ['Playfair Display', 'Georgia', 'serif'],
                        sans: ['Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>

    <!-- Google Fonts & FontAwesome -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,600;0,700;0,800;1,400&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0B0B0B;
            color: #F9F8F6;
            overflow-x: hidden;
        }

        /* Gold Gradient Text */
        .text-gold-gradient {
            background: linear-gradient(135deg, #E5C178 0%, #C5A059 50%, #9A7836 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* Luxury Gold Border Glow */
        .gold-border-glow {
            border: 1px solid rgba(197, 160, 89, 0.3);
            box-shadow: 0 0 20px rgba(197, 160, 89, 0.08);
        }

        .gold-border-glow:hover {
            border-color: rgba(197, 160, 89, 0.7);
            box-shadow: 0 0 25px rgba(197, 160, 89, 0.2);
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 7px;
        }
        ::-webkit-scrollbar-track {
            background: #0B0B0B;
        }
        ::-webkit-scrollbar-thumb {
            background: #262626;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #C5A059;
        }

        /* Subtle luxury overlay patterns */
        .bg-atelier-pattern {
            background-image: radial-gradient(circle at 1px 1px, rgba(197, 160, 89, 0.08) 1px, transparent 0);
            background-size: 32px 32px;
        }
    </style>
</head>
<body class="antialiased selection:bg-gold selection:text-onyx bg-onyx text-ivory">

    <!-- ==================== HEADER / NAVIGATION ==================== -->
    <header id="header" class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 bg-onyx/90 backdrop-blur-md border-b border-neutral-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            
            <!-- Atelier Wordmark -->
            <a href="#home" class="flex flex-col group focus:outline-none">
                <span class="font-serif text-lg sm:text-xl font-bold tracking-[0.2em] text-ivory group-hover:text-gold transition-colors">PAUL KABON</span>
                <span class="text-[9px] font-sans tracking-[0.35em] text-gold uppercase -mt-1">LUXURY ATELIER</span>
            </a>

            <!-- Desktop Nav Links -->
            <nav class="hidden md:flex items-center space-x-8 text-xs tracking-widest uppercase font-medium text-neutral-300">
                <a href="#home" class="hover:text-gold transition-colors duration-200">Home</a>
                <a href="#collections" class="hover:text-gold transition-colors duration-200">Collections</a>
                <a href="#shop" class="hover:text-gold transition-colors duration-200">Shop</a>
                <a href="#custom" class="hover:text-gold transition-colors duration-200">Custom Orders</a>
                <a href="#craft" class="hover:text-gold transition-colors duration-200">Our Craft</a>
                <a href="#story" class="hover:text-gold transition-colors duration-200">Story</a>
                <a href="#contact" class="hover:text-gold transition-colors duration-200">Contact</a>
            </nav>

            <!-- Action Buttons -->
            <div class="hidden md:flex items-center space-x-4">
                <a href="#shop" class="px-5 py-2.5 rounded-none border border-gold text-gold hover:bg-gold hover:text-onyx font-semibold text-xs tracking-widest uppercase transition-all duration-300">
                    Shop Collection
                </a>
            </div>

            <!-- Mobile Menu Button -->
            <button id="mobile-menu-btn" type="button" aria-label="Toggle Menu" class="md:hidden p-2 text-gold focus:outline-none">
                <i class="fa-solid fa-bars text-xl" id="menu-icon"></i>
            </button>
        </div>

        <!-- Mobile Drawer -->
        <div id="mobile-menu" class="hidden md:hidden bg-charcoal border-b border-neutral-800 px-6 pt-4 pb-8 space-y-4">
            <a href="#home" class="mobile-link block text-sm tracking-widest uppercase text-neutral-300 hover:text-gold">Home</a>
            <a href="#collections" class="mobile-link block text-sm tracking-widest uppercase text-neutral-300 hover:text-gold">Collections</a>
            <a href="#shop" class="mobile-link block text-sm tracking-widest uppercase text-neutral-300 hover:text-gold">Shop Catalogue</a>
            <a href="#custom" class="mobile-link block text-sm tracking-widest uppercase text-neutral-300 hover:text-gold">Custom Bespoke</a>
            <a href="#craft" class="mobile-link block text-sm tracking-widest uppercase text-neutral-300 hover:text-gold">Our Craftsmanship</a>
            <a href="#story" class="mobile-link block text-sm tracking-widest uppercase text-neutral-300 hover:text-gold">Our Story</a>
            <a href="#contact" class="mobile-link block text-sm tracking-widest uppercase text-neutral-300 hover:text-gold">Contact</a>
            
            <div class="pt-4 border-t border-neutral-800">
                <a href="https://wa.me/2349039916469?text=Hello%20Paul%20Kabon%20Luxury%20Atelier%2C%20I%20would%20like%20to%20inquire%20about%20your%20luxury%20leather%20collection." 
                   target="_blank" rel="noopener noreferrer" 
                   class="w-full py-3 bg-gold text-onyx font-bold text-xs tracking-widest uppercase text-center block">
                   <i class="fa-brands fa-whatsapp mr-1 text-sm"></i> WhatsApp Concierge
                </a>
            </div>
        </div>
    </header>

    <main class="pt-20">

        <!-- ==================== HERO SECTION ==================== -->
        <section id="home" class="relative min-h-[90vh] flex items-center bg-atelier-pattern overflow-hidden border-b border-neutral-800">
            <!-- Background Glow Decor -->
            <div class="absolute top-1/3 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[500px] h-[500px] bg-gold/5 blur-[120px] rounded-full pointer-events-none"></div>

            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16 lg:py-24 relative z-10">
                <div class="grid lg:grid-cols-12 gap-12 items-center">
                    
                    <!-- Left Hero Content -->
                    <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                        <div class="inline-flex items-center gap-3 px-3.5 py-1.5 border border-gold/30 bg-gold/5 text-gold text-xs tracking-[0.25em] uppercase font-medium">
                            <span class="w-1.5 h-1.5 bg-gold rounded-full"></span>
                            <span>Handmade in Awka, Nigeria</span>
                        </div>

                        <h1 class="text-3xl sm:text-5xl lg:text-6xl font-serif font-normal leading-tight tracking-tight text-ivory">
                            The Art of Fine <br class="hidden sm:inline" />
                            <span class="text-gold-gradient font-semibold italic">Leather Craftsmanship.</span>
                        </h1>

                        <p class="text-neutral-400 text-sm sm:text-base max-w-xl mx-auto lg:mx-0 font-light leading-relaxed">
                            Discover thoughtfully crafted leather footwear and accessories, made for those who appreciate quality, character, and timeless style.
                        </p>

                        <div class="pt-4 flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4">
                            <a href="#shop" class="w-full sm:w-auto px-8 py-4 bg-gold hover:bg-gold-light text-onyx font-semibold text-xs tracking-[0.2em] uppercase transition-all duration-300 text-center shadow-lg">
                                Explore The Collection
                            </a>
                            <a href="https://wa.me/2349039916469?text=Hello%20Paul%20Kabon%20Luxury%20Atelier%2C%20I%20am%20interested%20in%20discussing%20a%20custom%20bespoke%20leather%20order." 
                               target="_blank" rel="noopener noreferrer" 
                               class="w-full sm:w-auto px-8 py-4 border border-neutral-700 hover:border-gold text-ivory hover:text-gold font-semibold text-xs tracking-[0.2em] uppercase transition-all duration-300 text-center flex items-center justify-center gap-2">
                                <i class="fa-brands fa-whatsapp text-emerald-500 text-sm"></i>
                                <span>Customise Your Order</span>
                            </a>
                        </div>

                        <!-- Brand Statement Bar -->
                        <div class="pt-10 border-t border-neutral-800 grid grid-cols-3 gap-4 text-center lg:text-left">
                            <div>
                                <p class="text-[10px] tracking-widest uppercase text-gold font-bold">Materials</p>
                                <p class="text-xs text-neutral-300 mt-1">Full-Grain Leather</p>
                            </div>
                            <div>
                                <p class="text-[10px] tracking-widest uppercase text-gold font-bold">Process</p>
                                <p class="text-xs text-neutral-300 mt-1">Hand-Stitching</p>
                            </div>
                            <div>
                                <p class="text-[10px] tracking-widest uppercase text-gold font-bold">Service</p>
                                <p class="text-xs text-neutral-300 mt-1">Bespoke Fitting</p>
                            </div>
                        </div>
                    </div>

                    <!-- Right Visual Showcase Graphic -->
                    <div class="lg:col-span-5">
                        <div class="relative mx-auto max-w-md lg:max-w-none">
                            
                            <!-- Main Luxury Showcase Card -->
                            <div class="bg-charcoal p-6 rounded-none border border-gold/30 shadow-2xl relative">
                                <div class="relative h-80 sm:h-96 w-full bg-neutral-900 border border-neutral-800 flex flex-col justify-between p-6 overflow-hidden group">
                                    
                                    <!-- Decorative SVG Leather Craft Pattern Graphic -->
                                    <div class="absolute inset-0 opacity-15 flex items-center justify-center pointer-events-none">
                                        <svg width="240" height="240" viewBox="0 0 240 240" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <circle cx="120" cy="120" r="100" stroke="#C5A059" stroke-width="1" stroke-dasharray="4 4"/>
                                            <path d="M120 40 L120 200 M40 120 L200 120" stroke="#C5A059" stroke-width="0.5"/>
                                            <rect x="70" y="70" width="100" height="100" stroke="#C5A059" stroke-width="1"/>
                                        </svg>
                                    </div>

                                    <div class="flex justify-between items-start z-10">
                                        <span class="text-[10px] tracking-[0.3em] uppercase text-gold border border-gold/40 px-2.5 py-1 bg-onyx/80">
                                            ATELIER SPECIMEN
                                        </span>
                                        <span class="text-xs text-neutral-400 font-serif italic">Craft No. 01</span>
                                    </div>

                                    <!-- Graphic Artwork Representing Handmade Luxury Footwear & Bag -->
                                    <div class="text-center z-10 my-auto space-y-3">
                                        <div class="w-20 h-20 mx-auto rounded-full bg-gold/10 border border-gold/30 flex items-center justify-center text-gold text-3xl">
                                            <i class="fa-solid fa-gem"></i>
                                        </div>
                                        <h3 class="font-serif text-2xl text-ivory tracking-wide">Signature Collection</h3>
                                        <p class="text-xs text-neutral-400 font-light italic max-w-xs mx-auto">
                                            Hand-burnished Oxford shoes, structured leather portfolios, and custom dress belts.
                                        </p>
                                    </div>

                                    <div class="flex justify-between items-end text-[10px] tracking-widest text-gold uppercase border-t border-neutral-800 pt-3 z-10">
                                        <span>PAUL KABON</span>
                                        <span>PREMIUM NIGERIAN CRAFT</span>
                                    </div>
                                </div>

                                <div class="mt-4 flex items-center justify-between text-xs text-neutral-400 px-1">
                                    <span class="flex items-center gap-2"><i class="fa-solid fa-shield-halved text-gold"></i> Guaranteed Craftsmanship</span>
                                    <a href="#shop" class="text-gold hover:underline font-medium">Browse Stock &rarr;</a>
                                </div>
                            </div>

                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- ==================== FEATURED COLLECTIONS ==================== -->
        <section id="collections" class="py-20 bg-onyx border-b border-neutral-800">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                
                <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
                    <span class="text-[10px] font-bold uppercase tracking-[0.3em] text-gold">Curated Categories</span>
                    <h2 class="text-3xl sm:text-4xl font-serif text-ivory">Explore Our Collections</h2>
                    <p class="text-neutral-400 text-xs sm:text-sm font-light">Elegantly designed for daily refinement, formal occasions, and custom statements.</p>
                </div>

                <!-- 4 Collection Cards Grid -->
                <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-6">
                    
                    <!-- Collection 1: Shoes -->
                    <div class="bg-charcoal p-6 border border-neutral-800 hover:border-gold/50 transition-all duration-300 flex flex-col justify-between group">
                        <div class="space-y-4">
                            <div class="w-12 h-12 bg-onyx border border-neutral-700 flex items-center justify-center text-gold text-xl group-hover:border-gold transition-colors">
                                <i class="fa-solid fa-shoe-prints"></i>
                            </div>
                            <h3 class="text-lg font-serif text-ivory group-hover:text-gold transition-colors">Leather Shoes</h3>
                            <p class="text-neutral-400 text-xs font-light leading-relaxed">
                                Handmade footwear including Oxfords, Loafers, Monkstraps, and Chelsea boots designed for elegance and comfort.
                            </p>
                        </div>
                        <div class="pt-6 border-t border-neutral-800/80 mt-6">
                            <button onclick="filterCategory('Shoes')" class="text-xs font-semibold uppercase tracking-widest text-gold flex items-center gap-2 group-hover:translate-x-1 transition-transform">
                                <span>Explore Shoes</span>
                                <i class="fa-solid fa-arrow-right text-[10px]"></i>
                            </button>
                        </div>
                    </div>

                    <!-- Collection 2: Bags -->
                    <div class="bg-charcoal p-6 border border-neutral-800 hover:border-gold/50 transition-all duration-300 flex flex-col justify-between group">
                        <div class="space-y-4">
                            <div class="w-12 h-12 bg-onyx border border-neutral-700 flex items-center justify-center text-gold text-xl group-hover:border-gold transition-colors">
                                <i class="fa-solid fa-briefcase"></i>
                            </div>
                            <h3 class="text-lg font-serif text-ivory group-hover:text-gold transition-colors">Leather Bags</h3>
                            <p class="text-neutral-400 text-xs font-light leading-relaxed">
                                Executive portfolios, weekend duffel bags, structured totes, and slim document holders built with durability.
                            </p>
                        </div>
                        <div class="pt-6 border-t border-neutral-800/80 mt-6">
                            <button onclick="filterCategory('Bags')" class="text-xs font-semibold uppercase tracking-widest text-gold flex items-center gap-2 group-hover:translate-x-1 transition-transform">
                                <span>Explore Bags</span>
                                <i class="fa-solid fa-arrow-right text-[10px]"></i>
                            </button>
                        </div>
                    </div>

                    <!-- Collection 3: Belts -->
                    <div class="bg-charcoal p-6 border border-neutral-800 hover:border-gold/50 transition-all duration-300 flex flex-col justify-between group">
                        <div class="space-y-4">
                            <div class="w-12 h-12 bg-onyx border border-neutral-700 flex items-center justify-center text-gold text-xl group-hover:border-gold transition-colors">
                                <i class="fa-solid fa-ruler-horizontal"></i>
                            </div>
                            <h3 class="text-lg font-serif text-ivory group-hover:text-gold transition-colors">Refined Belts</h3>
                            <p class="text-neutral-400 text-xs font-light leading-relaxed">
                                Tailored full-grain leather belts with brass and silver buckles that complement suit tailoring and casual wear.
                            </p>
                        </div>
                        <div class="pt-6 border-t border-neutral-800/80 mt-6">
                            <button onclick="filterCategory('Belts')" class="text-xs font-semibold uppercase tracking-widest text-gold flex items-center gap-2 group-hover:translate-x-1 transition-transform">
                                <span>Explore Belts</span>
                                <i class="fa-solid fa-arrow-right text-[10px]"></i>
                            </button>
                        </div>
                    </div>

                    <!-- Collection 4: Custom Pieces -->
                    <div class="bg-charcoal p-6 border border-neutral-800 hover:border-gold/50 transition-all duration-300 flex flex-col justify-between group">
                        <div class="space-y-4">
                            <div class="w-12 h-12 bg-onyx border border-neutral-700 flex items-center justify-center text-gold text-xl group-hover:border-gold transition-colors">
                                <i class="fa-solid fa-pen-ruler"></i>
                            </div>
                            <h3 class="text-lg font-serif text-ivory group-hover:text-gold transition-colors">Custom Pieces</h3>
                            <p class="text-neutral-400 text-xs font-light leading-relaxed">
                                Personalised leather craft tailored to your distinct measurements, preferred hide colors, and design vision.
                            </p>
                        </div>
                        <div class="pt-6 border-t border-neutral-800/80 mt-6">
                            <a href="#custom" class="text-xs font-semibold uppercase tracking-widest text-gold flex items-center gap-2 group-hover:translate-x-1 transition-transform">
                                <span>Request Bespoke</span>
                                <i class="fa-solid fa-arrow-right text-[10px]"></i>
                            </a>
                        </div>
                    </div>

                </div>

            </div>
        </section>

        <!-- ==================== SHOP / PRODUCT CATALOGUE ==================== -->
        <section id="shop" class="py-20 bg-neutral-950 border-b border-neutral-800">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                
                <div class="flex flex-col md:flex-row md:items-end justify-between mb-12 gap-6">
                    <div class="space-y-2">
                        <span class="text-[10px] font-bold uppercase tracking-[0.3em] text-gold">Atelier Selection</span>
                        <h2 class="text-3xl sm:text-4xl font-serif text-ivory">Our Signature Pieces</h2>
                        <p class="text-neutral-400 text-xs sm:text-sm font-light">Explore handcrafted footwear and leather goods available for order.</p>
                    </div>

                    <!-- Filter Controls -->
                    <div class="flex flex-wrap items-center gap-2">
                        <button onclick="filterCategory('All')" class="filter-btn active px-4 py-2 text-xs font-semibold tracking-wider uppercase border border-gold bg-gold text-onyx transition-all" data-category="All">All</button>
                        <button onclick="filterCategory('Shoes')" class="filter-btn px-4 py-2 text-xs font-semibold tracking-wider uppercase border border-neutral-800 text-neutral-300 hover:border-gold transition-all" data-category="Shoes">Shoes</button>
                        <button onclick="filterCategory('Bags')" class="filter-btn px-4 py-2 text-xs font-semibold tracking-wider uppercase border border-neutral-800 text-neutral-300 hover:border-gold transition-all" data-category="Bags">Bags</button>
                        <button onclick="filterCategory('Belts')" class="filter-btn px-4 py-2 text-xs font-semibold tracking-wider uppercase border border-neutral-800 text-neutral-300 hover:border-gold transition-all" data-category="Belts">Belts</button>
                        <button onclick="filterCategory('Custom')" class="filter-btn px-4 py-2 text-xs font-semibold tracking-wider uppercase border border-neutral-800 text-neutral-300 hover:border-gold transition-all" data-category="Custom">Custom</button>
                    </div>
                </div>

                <!-- Product Grid -->
                <div id="product-grid" class="grid sm:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Dynamic Product Cards Injected via JS -->
                </div>

            </div>
        </section>

        <!-- ==================== CUSTOM ORDERS (MADE FOR YOU) ==================== -->
        <section id="custom" class="py-20 bg-onyx border-b border-neutral-800 bg-atelier-pattern">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                
                <div class="grid lg:grid-cols-12 gap-12 items-center">
                    
                    <!-- Left Copy -->
                    <div class="lg:col-span-5 space-y-6">
                        <span class="text-[10px] font-bold uppercase tracking-[0.3em] text-gold">Bespoke Service</span>
                        <h2 class="text-3xl sm:text-4xl font-serif text-ivory">Made for You</h2>
                        <p class="text-neutral-300 text-sm font-light leading-relaxed">
                            Every customer has a distinct style. Tell us what you have in mind, and let's discuss a leather piece tailored to your preferences.
                        </p>

                        <div class="space-y-4 text-xs text-neutral-400 border-t border-neutral-800 pt-6">
                            <div class="flex items-start gap-3">
                                <i class="fa-solid fa-compass-drafting text-gold text-base mt-0.5"></i>
                                <div>
                                    <h4 class="font-bold text-ivory uppercase tracking-wider text-[11px]">Custom Measurements</h4>
                                    <p class="mt-0.5">Foot sizing, strap lengths, and interior compartment specifications.</p>
                                </div>
                            </div>
                            <div class="flex items-start gap-3">
                                <i class="fa-solid fa-palette text-gold text-base mt-0.5"></i>
                                <div>
                                    <h4 class="font-bold text-ivory uppercase tracking-wider text-[11px]">Leather & Color Options</h4>
                                    <p class="mt-0.5">Select from Cognac Brown, Espresso Dark Tan, Onyx Black, or Burgundy hides.</p>
                                </div>
                            </div>
                            <div class="flex items-start gap-3">
                                <i class="fa-solid fa-comments text-gold text-base mt-0.5"></i>
                                <div>
                                    <h4 class="font-bold text-ivory uppercase tracking-wider text-[11px]">Direct Artisan Consultation</h4>
                                    <p class="mt-0.5">Direct chat via WhatsApp to refine drawings, budget, and timeline.</p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Right Custom Order Form -->
                    <div class="lg:col-span-7">
                        <div class="bg-charcoal p-6 sm:p-8 border border-gold/30 shadow-2xl">
                            <h3 class="text-xl font-serif text-ivory mb-6 border-b border-neutral-800 pb-3">Request a Custom Design</h3>
                            
                            <form id="custom-order-form" class="space-y-4 text-xs">
                                <div class="grid sm:grid-cols-2 gap-4">
                                    <div>
                                        <label for="custName" class="block text-[10px] uppercase font-bold tracking-widest text-gold mb-1">Your Name *</label>
                                        <input type="text" id="custName" required placeholder="e.g. Alex Morgan" class="w-full px-4 py-3 bg-onyx border border-neutral-700 text-ivory focus:outline-none focus:border-gold">
                                    </div>
                                    <div>
                                        <label for="productType" class="block text-[10px] uppercase font-bold tracking-widest text-gold mb-1">Product Type *</label>
                                        <select id="productType" required class="w-full px-4 py-3 bg-onyx border border-neutral-700 text-ivory focus:outline-none focus:border-gold">
                                            <option value="">Select Category...</option>
                                            <option value="Bespoke Shoes / Boots">Bespoke Shoes / Boots</option>
                                            <option value="Custom Leather Bag / Portfolio">Custom Leather Bag / Portfolio</option>
                                            <option value="Tailored Dress Belt">Tailored Dress Belt</option>
                                            <option value="Matching Accessory Set">Matching Accessory Set</option>
                                        </select>
                                    </div>
                                </div>

                                <div class="grid sm:grid-cols-2 gap-4">
                                    <div>
                                        <label for="colorPref" class="block text-[10px] uppercase font-bold tracking-widest text-gold mb-1">Preferred Leather Color</label>
                                        <input type="text" id="colorPref" placeholder="e.g. Dark Tan, Onyx Black, Mahogany" class="w-full px-4 py-3 bg-onyx border border-neutral-700 text-ivory focus:outline-none focus:border-gold">
                                    </div>
                                    <div>
                                        <label for="sizePref" class="block text-[10px] uppercase font-bold tracking-widest text-gold mb-1">Shoe Size / Measurements</label>
                                        <input type="text" id="sizePref" placeholder="e.g. EU 43 / Waist 34 / Standard" class="w-full px-4 py-3 bg-onyx border border-neutral-700 text-ivory focus:outline-none focus:border-gold">
                                    </div>
                                </div>

                                <div>
                                    <label for="designDesc" class="block text-[10px] uppercase font-bold tracking-widest text-gold mb-1">Design Description & Details *</label>
                                    <textarea id="designDesc" rows="3" required placeholder="Describe what you want us to craft (style preferences, sole type, stitching detail...)" class="w-full px-4 py-3 bg-onyx border border-neutral-700 text-ivory focus:outline-none focus:border-gold"></textarea>
                                </div>

                                <div>
                                    <label for="budgetRange" class="block text-[10px] uppercase font-bold tracking-widest text-gold mb-1">Estimated Budget Range (Optional)</label>
                                    <input type="text" id="budgetRange" placeholder="e.g. ₦60,000 - ₦150,000" class="w-full px-4 py-3 bg-onyx border border-neutral-700 text-ivory focus:outline-none focus:border-gold">
                                </div>

                                <p id="custom-form-error" class="text-rose-500 font-semibold text-[11px] hidden"></p>

                                <button type="submit" class="w-full py-4 bg-gold hover:bg-gold-light text-onyx font-bold text-xs tracking-[0.2em] uppercase transition-all shadow-md flex items-center justify-center gap-2">
                                    <i class="fa-brands fa-whatsapp text-sm"></i>
                                    <span>Send Custom Request on WhatsApp</span>
                                </button>
                                <p class="text-[10px] text-neutral-500 text-center">Submitting will compile your specifications into WhatsApp to message our master craftsman directly.</p>
                            </form>
                        </div>
                    </div>

                </div>

            </div>
        </section>

        <!-- ==================== OUR CRAFTSMANSHIP ==================== -->
        <section id="craft" class="py-20 bg-neutral-950 border-b border-neutral-800">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                
                <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
                    <span class="text-[10px] font-bold uppercase tracking-[0.3em] text-gold">Artisanal Process</span>
                    <h2 class="text-3xl sm:text-4xl font-serif text-ivory">Crafted by Hand. Finished with Care.</h2>
                    <p class="text-neutral-400 text-xs sm:text-sm font-light">Every piece undergoes a multi-stage hand-finishing process to guarantee longevity.</p>
                </div>

                <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-6">
                    
                    <!-- Stage 1 -->
                    <div class="bg-charcoal p-6 border border-neutral-800 relative space-y-3">
                        <span class="text-gold font-serif text-2xl font-bold">01</span>
                        <h3 class="text-base font-serif text-ivory">Material Selection</h3>
                        <p class="text-neutral-400 text-xs font-light leading-relaxed">
                            Carefully evaluating full-grain leather hides for grain consistency, durability, and texture before cutting begins.
                        </p>
                    </div>

                    <!-- Stage 2 -->
                    <div class="bg-charcoal p-6 border border-neutral-800 relative space-y-3">
                        <span class="text-gold font-serif text-2xl font-bold">02</span>
                        <h3 class="text-base font-serif text-ivory">Precision Cutting</h3>
                        <p class="text-neutral-400 text-xs font-light leading-relaxed">
                            Hand-patterning and blade cutting leather panels to preserve strength along natural structural lines.
                        </p>
                    </div>

                    <!-- Stage 3 -->
                    <div class="bg-charcoal p-6 border border-neutral-800 relative space-y-3">
                        <span class="text-gold font-serif text-2xl font-bold">03</span>
                        <h3 class="text-base font-serif text-ivory">Hand Stitching</h3>
                        <p class="text-neutral-400 text-xs font-light leading-relaxed">
                            Reinforced hand stitching and edge painting using wax-treated threads designed to withstand daily wear.
                        </p>
                    </div>

                    <!-- Stage 4 -->
                    <div class="bg-charcoal p-6 border border-neutral-800 relative space-y-3">
                        <span class="text-gold font-serif text-2xl font-bold">04</span>
                        <h3 class="text-base font-serif text-ivory">Lasting & Finish</h3>
                        <p class="text-neutral-400 text-xs font-light leading-relaxed">
                            Shaping over lasts, applying cream polishes, edge burnishing, and final quality inspection before client delivery.
                        </p>
                    </div>

                </div>

            </div>
        </section>

        <!-- ==================== ABOUT THE BRAND / STORY ==================== -->
        <section id="story" class="py-20 bg-onyx border-b border-neutral-800">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="grid lg:grid-cols-12 gap-12 items-center">
                    
                    <div class="lg:col-span-6 space-y-6">
                        <span class="text-[10px] font-bold uppercase tracking-[0.3em] text-gold">The Atelier Heritage</span>
                        <h2 class="text-3xl sm:text-4xl font-serif text-ivory">The Paul Kabon Story</h2>
                        
                        <p class="text-neutral-300 text-sm leading-relaxed font-light">
                            Paul Kabon Luxury Atelier is a leather fashion brand dedicated to creating distinctive footwear and accessories for customers who appreciate craftsmanship, thoughtful design, and quality. Our focus is on leather pieces that combine style, function, and attention to detail.
                        </p>

                        <p class="text-neutral-400 text-xs leading-relaxed font-light">
                            Operating from Awka, Anambra State, Nigeria, each creation balances classic leatherwork with modern aesthetics, ensuring our clients receive long-lasting pieces crafted with purpose.
                        </p>

                        <div class="pt-4 border-t border-neutral-800 flex items-center gap-6 text-xs text-neutral-400">
                            <div>
                                <span class="block font-bold text-gold text-base">Awka, Nigeria</span>
                                <span class="text-[10px] uppercase tracking-wider">Atelier Location</span>
                            </div>
                            <div class="h-8 w-px bg-neutral-800"></div>
                            <div>
                                <span class="block font-bold text-gold text-base">100% Leather</span>
                                <span class="text-[10px] uppercase tracking-wider">Genuine Crafts</span>
                            </div>
                        </div>
                    </div>

                    <!-- Right Column: Atelier Pillars Grid -->
                    <div class="lg:col-span-6 grid sm:grid-cols-2 gap-4">
                        <div class="bg-charcoal p-6 border border-neutral-800 space-y-2">
                            <i class="fa-solid fa-gem text-gold text-xl"></i>
                            <h4 class="font-serif text-ivory text-sm">Attention to Detail</h4>
                            <p class="text-neutral-400 text-xs font-light">Thoughtful finishing, clean edge painting, and careful presentation.</p>
                        </div>

                        <div class="bg-charcoal p-6 border border-neutral-800 space-y-2">
                            <i class="fa-solid fa-crown text-gold text-xl"></i>
                            <h4 class="font-serif text-ivory text-sm">Distinctive Style</h4>
                            <p class="text-neutral-400 text-xs font-light">Leather pieces with individual character and refined aesthetic appeal.</p>
                        </div>

                        <div class="bg-charcoal p-6 border border-neutral-800 space-y-2">
                            <i class="fa-solid fa-handshake-angle text-gold text-xl"></i>
                            <h4 class="font-serif text-ivory text-sm">Personalised Service</h4>
                            <p class="text-neutral-400 text-xs font-light">Direct communication for product inquiries and custom bespoke requests.</p>
                        </div>

                        <div class="bg-charcoal p-6 border border-neutral-800 space-y-2">
                            <i class="fa-solid fa-hammer text-gold text-xl"></i>
                            <h4 class="font-serif text-ivory text-sm">Craftsmanship</h4>
                            <p class="text-neutral-400 text-xs font-light">Uncompromised focus on the labor, skill, and tradition behind each hide.</p>
                        </div>
                    </div>

                </div>
            </div>
        </section>

        <!-- ==================== CONTACT AND CUSTOMER CARE ==================== -->
        <section id="contact" class="py-20 bg-neutral-950">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                
                <div class="grid lg:grid-cols-12 gap-12">
                    
                    <!-- Left Contact Info -->
                    <div class="lg:col-span-5 space-y-6">
                        <div>
                            <span class="text-[10px] font-bold uppercase tracking-[0.3em] text-gold">Concierge Care</span>
                            <h2 class="text-3xl sm:text-4xl font-serif text-ivory">Let's Find Your Next Signature Piece</h2>
                            <p class="text-neutral-400 text-xs sm:text-sm mt-3 font-light leading-relaxed">
                                Connect directly with our atelier for stock availability, bespoke requests, size consultations, or custom leather commissions.
                            </p>
                        </div>

                        <div class="space-y-4 text-xs">
                            <!-- WhatsApp -->
                            <a href="https://wa.me/2349039916469" target="_blank" rel="noopener noreferrer" class="flex items-center gap-4 p-4 bg-charcoal border border-neutral-800 hover:border-gold transition-colors">
                                <div class="w-10 h-10 bg-onyx text-emerald-500 border border-neutral-700 flex items-center justify-center text-lg">
                                    <i class="fa-brands fa-whatsapp"></i>
                                </div>
                                <div>
                                    <p class="text-[10px] uppercase tracking-wider text-neutral-400 font-semibold">WhatsApp Concierge</p>
                                    <p class="font-bold text-ivory text-sm">+234 903 991 6469</p>
                                </div>
                            </a>

                            <!-- Email -->
                            <a href="mailto:paulkabon8@gmail.com" class="flex items-center gap-4 p-4 bg-charcoal border border-neutral-800 hover:border-gold transition-colors">
                                <div class="w-10 h-10 bg-onyx text-gold border border-neutral-700 flex items-center justify-center text-lg">
                                    <i class="fa-solid fa-envelope"></i>
                                </div>
                                <div>
                                    <p class="text-[10px] uppercase tracking-wider text-neutral-400 font-semibold">Email Inquiry</p>
                                    <p class="font-bold text-ivory text-sm">paulkabon8@gmail.com</p>
                                </div>
                            </a>

                            <!-- Location -->
                            <div class="flex items-center gap-4 p-4 bg-charcoal border border-neutral-800">
                                <div class="w-10 h-10 bg-onyx text-gold border border-neutral-700 flex items-center justify-center text-lg">
                                    <i class="fa-solid fa-location-dot"></i>
                                </div>
                                <div>
                                    <p class="text-[10px] uppercase tracking-wider text-neutral-400 font-semibold">Atelier Location</p>
                                    <p class="font-bold text-ivory text-sm">Awka, Anambra State, Nigeria</p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Right Quick Form -->
                    <div class="lg:col-span-7">
                        <div class="bg-charcoal p-6 sm:p-8 border border-neutral-800">
                            <h3 class="text-xl font-serif text-ivory mb-6 border-b border-neutral-800 pb-3">Send an Inquiry</h3>
                            
                            <form id="contact-inquiry-form" class="space-y-4 text-xs">
                                <div class="grid sm:grid-cols-2 gap-4">
                                    <div>
                                        <label for="contactName" class="block text-[10px] uppercase font-bold tracking-widest text-gold mb-1">Full Name *</label>
                                        <input type="text" id="contactName" required placeholder="e.g. David O." class="w-full px-4 py-3 bg-onyx border border-neutral-700 text-ivory focus:outline-none focus:border-gold">
                                    </div>
                                    <div>
                                        <label for="contactEmail" class="block text-[10px] uppercase font-bold tracking-widest text-gold mb-1">Email Address *</label>
                                        <input type="email" id="contactEmail" required placeholder="e.g. david@example.com" class="w-full px-4 py-3 bg-onyx border border-neutral-700 text-ivory focus:outline-none focus:border-gold">
                                    </div>
                                </div>

                                <div>
                                    <label for="contactMessage" class="block text-[10px] uppercase font-bold tracking-widest text-gold mb-1">Message / Question *</label>
                                    <textarea id="contactMessage" rows="4" required placeholder="Inquire about shoe sizes, bag customization, or pricing details..." class="w-full px-4 py-3 bg-onyx border border-neutral-700 text-ivory focus:outline-none focus:border-gold"></textarea>
                                </div>

                                <button type="submit" class="w-full py-4 bg-gold hover:bg-gold-light text-onyx font-bold text-xs tracking-[0.2em] uppercase transition-all flex items-center justify-center gap-2">
                                    <i class="fa-brands fa-whatsapp text-sm"></i>
                                    <span>Send Message via WhatsApp</span>
                                </button>
                            </form>
                        </div>
                    </div>

                </div>

            </div>
        </section>

    </main>

    <!-- ==================== FOOTER ==================== -->
    <footer class="bg-onyx border-t border-neutral-800 text-neutral-400 py-12 text-xs">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-8 mb-12">
                
                <!-- Brand Col -->
                <div class="space-y-3">
                    <div class="flex flex-col">
                        <span class="font-serif text-lg font-bold tracking-[0.2em] text-ivory">PAUL KABON</span>
                        <span class="text-[9px] tracking-[0.35em] text-gold uppercase -mt-1">LUXURY ATELIER</span>
                    </div>
                    <p class="text-neutral-400 text-xs font-light leading-relaxed">
                        Crafted with Precision. Designed with Purpose.
                    </p>
                </div>

                <!-- Navigation -->
                <div>
                    <h4 class="text-[10px] font-bold uppercase tracking-widest text-gold mb-3">Navigation</h4>
                    <ul class="space-y-2">
                        <li><a href="#home" class="hover:text-gold transition-colors">Home</a></li>
                        <li><a href="#collections" class="hover:text-gold transition-colors">Collections</a></li>
                        <li><a href="#shop" class="hover:text-gold transition-colors">Signature Shop</a></li>
                        <li><a href="#custom" class="hover:text-gold transition-colors">Custom Orders</a></li>
                        <li><a href="#craft" class="hover:text-gold transition-colors">Our Craft</a></li>
                    </ul>
                </div>

                <!-- Categories -->
                <div>
                    <h4 class="text-[10px] font-bold uppercase tracking-widest text-gold mb-3">Leather Categories</h4>
                    <ul class="space-y-2">
                        <li><button onclick="filterCategory('Shoes')" class="hover:text-gold transition-colors text-left">Handmade Footwear</button></li>
                        <li><button onclick="filterCategory('Bags')" class="hover:text-gold transition-colors text-left">Executive Portfolios & Bags</button></li>
                        <li><button onclick="filterCategory('Belts')" class="hover:text-gold transition-colors text-left">Full-Grain Dress Belts</button></li>
                        <li><a href="#custom" class="hover:text-gold transition-colors">Bespoke Custom Orders</a></li>
                    </ul>
                </div>

                <!-- Direct WhatsApp Hotline -->
                <div>
                    <h4 class="text-[10px] font-bold uppercase tracking-widest text-gold mb-3">Direct Hotline</h4>
                    <p class="mb-2">Awka, Anambra State, Nigeria</p>
                    <a href="https://wa.me/2349039916469" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-2 text-emerald-400 font-semibold hover:underline">
                        <i class="fa-brands fa-whatsapp text-sm"></i>
                        <span>+234 903 991 6469</span>
                    </a>
                </div>

            </div>

            <div class="pt-8 border-t border-neutral-800 flex flex-col sm:flex-row items-center justify-between text-neutral-500 text-[11px] gap-4">
                <p>&copy; <span id="copyright-year"></span> Paul Kabon Luxury Atelier. All rights reserved.</p>
                <p>Awka, Nigeria &bull; Fine Handmade Leatherwork</p>
            </div>
        </div>
    </footer>

    <!-- ==================== PRODUCT QUICK VIEW MODAL ==================== -->
    <div id="product-modal" class="fixed inset-0 bg-onyx/90 backdrop-blur-md z-50 hidden items-center justify-center p-4">
        <div class="bg-charcoal border border-gold/30 max-w-2xl w-full p-6 sm:p-8 relative shadow-2xl max-h-[90vh] overflow-y-auto">
            
            <button id="close-modal-btn" type="button" aria-label="Close modal" class="absolute top-4 right-4 text-neutral-400 hover:text-gold p-2 text-xl">
                <i class="fa-solid fa-xmark"></i>
            </button>

            <div id="modal-content" class="space-y-6">
                <!-- Dynamically populated product view -->
            </div>
        </div>
    </div>

    <!-- ==================== JAVASCRIPT ==================== -->
    <script>
        // Sample Signature Product Stock Data
        const productsData = [
            {
                id: 'shoe-01',
                name: 'The Royal Oxford Leather Shoe',
                category: 'Shoes',
                priceNaira: 85000,
                tag: 'Hand-Burnished',
                sizes: ['EU 40', 'EU 41', 'EU 42', 'EU 43', 'EU 44', 'EU 45'],
                colors: ['Espresso Brown', 'Onyx Black'],
                icon: 'fa-shoe-prints',
                description: 'Classic closed-lacing Oxford shoe crafted from premium calfskin leather hide. Hand-polished finish with durable stacked leather sole for corporate and black-tie elegance.'
            },
            {
                id: 'shoe-02',
                name: 'The Sovereign Penny Loafer',
                category: 'Shoes',
                priceNaira: 75000,
                tag: 'Slip-On Luxury',
                sizes: ['EU 40', 'EU 41', 'EU 42', 'EU 43', 'EU 44'],
                colors: ['Cognac Tan', 'Burgundy'],
                icon: 'fa-shoe-prints',
                description: 'Hand-stitched penny loafer designed for modern luxury and effortless slip-on comfort. Crafted with cushioned insoles for all-day elegance.'
            },
            {
                id: 'bag-01',
                name: 'The Atelier Executive Portfolio Bag',
                category: 'Bags',
                priceNaira: 120000,
                tag: 'Full Grain',
                sizes: ['15-inch Laptop Fit'],
                colors: ['Onyx Black', 'Dark Cognac'],
                icon: 'fa-briefcase',
                description: 'Structured document portfolio featuring brass hardware zippers, velvet lining, padded laptop sleeve, and detachable leather shoulder strap.'
            },
            {
                id: 'bag-02',
                name: 'The Voyager Leather Duffel Bag',
                category: 'Bags',
                priceNaira: 160000,
                tag: 'Travel Essential',
                sizes: ['Carry-On Capacity'],
                colors: ['Rich Mahogany', 'Espresso'],
                icon: 'fa-suitcase',
                description: 'Spacious leather weekend duffel bag with reinforced handles, brass studs, and heavy-duty stitching engineered for travel durability.'
            },
            {
                id: 'belt-01',
                name: 'The Artisan Tailored Dress Belt',
                category: 'Belts',
                priceNaira: 28000,
                tag: 'Full-Grain Leather',
                sizes: ['32', '34', '36', '38', '40', 'Custom Waist'],
                colors: ['Black', 'Tan', 'Dark Brown'],
                icon: 'fa-ruler-horizontal',
                description: 'Double-edge stitched dress belt made from thick full-grain leather hide, featuring solid brass or brushed chrome buckle options.'
            },
            {
                id: 'custom-01',
                name: 'Bespoke Monogrammed Footwear Set',
                category: 'Custom',
                priceNaira: 110000,
                tag: 'Made to Order',
                sizes: ['Custom Fitted'],
                colors: ['Client Selection'],
                icon: 'fa-gem',
                description: 'Fully personalized leather footwear crafted to your exact foot measurements with optional gold foil initials embossed on the sock lining.'
            }
        ];

        document.addEventListener('DOMContentLoaded', function () {
            
            // 1. Dynamic Copyright Year
            const copyYear = document.getElementById('copyright-year');
            if (copyYear) copyYear.textContent = new Date().getFullYear();

            // 2. Mobile Drawer
            const mobileBtn = document.getElementById('mobile-menu-btn');
            const mobileMenu = document.getElementById('mobile-menu');
            const menuIcon = document.getElementById('menu-icon');
            const mobileLinks = document.querySelectorAll('.mobile-link');

            if (mobileBtn && mobileMenu && menuIcon) {
                mobileBtn.addEventListener('click', function () {
                    mobileMenu.classList.toggle('hidden');
                    if (mobileMenu.classList.contains('hidden')) {
                        menuIcon.classList.remove('fa-xmark');
                        menuIcon.classList.add('fa-bars');
                    } else {
                        menuIcon.classList.remove('fa-bars');
                        menuIcon.classList.add('fa-xmark');
                    }
                });

                mobileLinks.forEach(link => {
                    link.addEventListener('click', () => {
                        mobileMenu.classList.add('hidden');
                        menuIcon.classList.remove('fa-xmark');
                        menuIcon.classList.add('fa-bars');
                    });
                });
            }

            // 3. Render Product Cards
            renderProducts('All');

            // 4. Modal Handlers
            const modal = document.getElementById('product-modal');
            const closeModalBtn = document.getElementById('close-modal-btn');
            
            if (closeModalBtn) {
                closeModalBtn.addEventListener('click', closeModal);
            }
            if (modal) {
                modal.addEventListener('click', function(e) {
                    if (e.target === modal) closeModal();
                });
            }

            // 5. Custom Order Form WhatsApp Formatting
            const customForm = document.getElementById('custom-order-form');
            if (customForm) {
                customForm.addEventListener('submit', function(e) {
                    e.preventDefault();
                    
                    const name = document.getElementById('custName').value.trim();
                    const productType = document.getElementById('productType').value;
                    const color = document.getElementById('colorPref').value.trim() || 'Not specified';
                    const size = document.getElementById('sizePref').value.trim() || 'Not specified';
                    const desc = document.getElementById('designDesc').value.trim();
                    const budget = document.getElementById('budgetRange').value.trim() || 'To be discussed';
                    const formErr = document.getElementById('custom-form-error');

                    if (!name || !productType || !desc) {
                        if (formErr) {
                            formErr.textContent = 'Please fill out all required fields marked with *';
                            formErr.classList.remove('hidden');
                        }
                        return;
                    }

                    if (formErr) formErr.classList.add('hidden');

                    const message = `Hello Paul Kabon Luxury Atelier,\n\nI would like to submit a Custom Bespoke Order Request:\n\n- Name: ${name}\n- Product Type: ${productType}\n- Preferred Color: ${color}\n- Size/Measurements: ${size}\n- Budget Range: ${budget}\n- Details: ${desc}`;

                    window.open(`https://wa.me/2349039916469?text=${encodeURIComponent(message)}`, '_blank');
                });
            }

            // 6. Contact Form Formatting
            const contactForm = document.getElementById('contact-inquiry-form');
            if (contactForm) {
                contactForm.addEventListener('submit', function(e) {
                    e.preventDefault();
                    
                    const name = document.getElementById('contactName').value.trim();
                    const email = document.getElementById('contactEmail').value.trim();
                    const msg = document.getElementById('contactMessage').value.trim();

                    if (!name || !email || !msg) return;

                    const text = `Hello Paul Kabon Luxury Atelier,\n\nI have an inquiry from your website:\n\n- Name: ${name}\n- Email: ${email}\n- Message: ${msg}`;
                    window.open(`https://wa.me/2349039916469?text=${encodeURIComponent(text)}`, '_blank');
                });
            }

        });

        // Filter Category Function
        function filterCategory(category) {
            const buttons = document.querySelectorAll('.filter-btn');
            buttons.forEach(btn => {
                if (btn.getAttribute('data-category') === category) {
                    btn.classList.add('bg-gold', 'text-onyx', 'border-gold');
                    btn.classList.remove('border-neutral-800', 'text-neutral-300');
                } else {
                    btn.classList.remove('bg-gold', 'text-onyx', 'border-gold');
                    btn.classList.add('border-neutral-800', 'text-neutral-300');
                }
            });

            renderProducts(category);
        }

        // Render Product Cards
        function renderProducts(filter) {
            const grid = document.getElementById('product-grid');
            if (!grid) return;

            grid.innerHTML = '';

            const filtered = filter === 'All' ? productsData : productsData.filter(p => p.category === filter);

            filtered.forEach(p => {
                const formattedPrice = `₦${p.priceNaira.toLocaleString()}`;
                
                const card = document.createElement('div');
                card.className = 'bg-charcoal border border-neutral-800 hover:border-gold/40 transition-all duration-300 p-5 flex flex-col justify-between group';
                
                card.innerHTML = `
                    <div class="space-y-4">
                        <div class="h-48 bg-neutral-900 border border-neutral-800 flex flex-col items-center justify-center p-4 relative group-hover:border-gold/30 transition-colors">
                            <span class="absolute top-3 left-3 text-[9px] uppercase tracking-widest text-gold border border-gold/30 px-2 py-0.5 bg-onyx/80">${p.tag}</span>
                            <i class="fa-solid ${p.icon} text-4xl text-gold/80 mb-2 group-hover:scale-110 transition-transform duration-300"></i>
                            <span class="text-[10px] text-neutral-500 uppercase tracking-widest font-mono">Paul Kabon Craft</span>
                        </div>

                        <div>
                            <span class="text-[9px] uppercase tracking-widest text-gold">${p.category}</span>
                            <h3 class="font-serif text-lg text-ivory group-hover:text-gold transition-colors mt-0.5">${p.name}</h3>
                            <p class="text-xs font-bold text-gold-gradient mt-1">${formattedPrice}</p>
                            <p class="text-neutral-400 text-xs font-light line-clamp-2 mt-2">${p.description}</p>
                        </div>
                    </div>

                    <div class="pt-4 border-t border-neutral-800/80 mt-6 grid grid-cols-2 gap-2">
                        <button onclick="openQuickView('${p.id}')" class="py-2.5 px-2 bg-neutral-900 hover:bg-neutral-800 text-neutral-300 hover:text-ivory border border-neutral-700 text-[10px] uppercase tracking-wider font-semibold text-center transition-colors">
                            Quick View
                        </button>
                        <a href="https://wa.me/2349039916469?text=${encodeURIComponent(`Hello Paul Kabon Luxury Atelier, I am interested in ordering: ${p.name} (${formattedPrice}). Please confirm availability.`)}" 
                           target="_blank" rel="noopener noreferrer" 
                           class="py-2.5 px-2 bg-gold hover:bg-gold-light text-onyx font-bold text-[10px] uppercase tracking-wider text-center flex items-center justify-center gap-1 transition-colors">
                            <i class="fa-brands fa-whatsapp"></i>
                            <span>Order</span>
                        </a>
                    </div>
                `;

                grid.appendChild(card);
            });
        }

        // Open Quick View Modal
        function openQuickView(productId) {
            const product = productsData.find(p => p.id === productId);
            if (!product) return;

            const modalContent = document.getElementById('modal-content');
            const modal = document.getElementById('product-modal');
            if (!modalContent || !modal) return;

            const formattedPrice = `₦${product.priceNaira.toLocaleString()}`;

            modalContent.innerHTML = `
                <div class="space-y-4">
                    <div class="inline-block px-2.5 py-1 border border-gold/30 bg-gold/5 text-gold text-[10px] uppercase tracking-widest">
                        ${product.category} &bull; ${product.tag}
                    </div>

                    <h3 class="text-2xl font-serif text-ivory">${product.name}</h3>
                    <p class="text-xl font-bold text-gold">${formattedPrice}</p>

                    <p class="text-xs text-neutral-300 leading-relaxed font-light">${product.description}</p>

                    <div class="space-y-2 border-t border-b border-neutral-800 py-4 text-xs">
                        <div>
                            <span class="text-[10px] uppercase tracking-widest text-gold font-bold">Available Sizes / Specs:</span>
                            <div class="flex flex-wrap gap-1.5 mt-1">
                                ${product.sizes.map(s => `<span class="px-2 py-1 bg-onyx border border-neutral-700 text-neutral-300 text-[10px]">${s}</span>`).join('')}
                            </div>
                        </div>

                        <div class="pt-2">
                            <span class="text-[10px] uppercase tracking-widest text-gold font-bold">Color Finishes:</span>
                            <p class="text-neutral-300 text-xs">${product.colors.join(', ')}</p>
                        </div>
                    </div>

                    <div class="pt-2 flex flex-col sm:flex-row gap-3">
                        <a href="https://wa.me/2349039916469?text=${encodeURIComponent(`Hello Paul Kabon Luxury Atelier, I want to order the ${product.name} priced at ${formattedPrice}. Let's discuss sizing and delivery.`)}" 
                           target="_blank" rel="noopener noreferrer" 
                           class="w-full py-3.5 bg-gold text-onyx font-bold text-xs uppercase tracking-widest text-center flex items-center justify-center gap-2">
                            <i class="fa-brands fa-whatsapp text-sm"></i>
                            <span>Order via WhatsApp Concierge</span>
                        </a>
                    </div>
                </div>
            `;

            modal.classList.remove('hidden');
            modal.classList.add('flex');
            document.body.style.overflow = 'hidden';
        }

        // Close Modal
        function closeModal() {
            const modal = document.getElementById('product-modal');
            if (modal) {
                modal.classList.add('hidden');
                modal.classList.remove('flex');
                document.body.style.overflow = '';
            }
        }
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SHOUPAY | Premium Fashion Brand</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .hero-section {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/5ac66ee5-7da2-497a-9bd2-5cba9221418c.png');
            background-size: cover;
            background-position: center;
            height: 80vh;
        }
        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }
        .product-card .product-actions {
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        .product-card:hover .product-actions {
            opacity: 1;
        }
        .dropdown:hover .dropdown-menu {
            display: block;
        }
        .size-selector input[type="radio"]:checked + label {
            background-color: black;
            color: white;
        }
        .cart-count {
            position: absolute;
            top: -8px;
            right: -8px;
            background-color: black;
            color: white;
            border-radius: 50%;
            width: 20px;
            height: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 12px;
        }
    </style>
</head>
<body class="bg-gray-50 font-sans">
    <!-- Header/Navbar -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-12">
                <a href="#" class="text-2xl font-bold tracking-tighter flex items-center">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/91625525-8d93-4d42-80e3-6f6c011dd6eb.png" alt="Premium fashion brand logo" class="h-5 mr-2">
                    SHOUPAY
                </a>
                <nav class="hidden md:flex space-x-8">
                    <div class="dropdown relative">
                        <button class="hover:text-gray-600 flex items-center">
                            New & Featured <i class="fas fa-chevron-down text-xs ml-1"></i>
                        </button>
                        <div class="dropdown-menu absolute hidden bg-white shadow-lg rounded-md py-2 w-48">
                            <a href="#" class="block px-4 py-2 hover:bg-gray-100">New Releases</a>
                            <a href="#" class="block px-4 py-2 hover:bg-gray-100">Best Sellers</a>
                            <a href="#" class="block px-4 py-2 hover:bg-gray-100">Member Access</a>
                        </div>
                    </div>
                    <div class="dropdown relative">
                        <button class="hover:text-gray-600 flex items-center">
                            Men <i class="fas fa-chevron-down text-xs ml-1"></i>
                        </button>
                        <div class="dropdown-menu absolute hidden bg-white shadow-xl rounded-md py-3 w-56 divide-y divide-gray-100">
                            <div class="px-4 py-2">
                                <h4 class="font-bold text-gray-800 mb-2">MEN'S</h4>
                                <a href="#" class="block px-2 py-2 hover:bg-gray-50 rounded">All Hoodies</a>
                                <a href="#" class="block px-2 py-2 hover:bg-gray-50 rounded">Premium Collection</a>
                                <a href="#" class="block px-2 py-2 hover:bg-gray-50 rounded">Graphic Prints</a>
                            </div>
                            <div class="px-4 py-2">
                                <h4 class="font-bold text-gray-800 mb-2">ESSENTIALS</h4>
                                <a href="#" class="block px-2 py-2 hover:bg-gray-50 rounded">T-Shirts</a>
                                <a href="#" class="block px-2 py-2 hover:bg-gray-50 rounded">Sweatshirts</a>
                                <a href="#" class="block px-2 py-2 hover:bg-gray-50 rounded">Joggers</a>
                            </div>
                        </div>
                    </div>
                    <div class="dropdown relative">
                        <button class="hover:text-gray-600 flex items-center">
                            Women <i class="fas fa-chevron-down text-xs ml-1"></i>
                        </button>
                        <div class="dropdown-menu absolute hidden bg-white shadow-lg rounded-md py-2 w-48">
                            <a href="#" class="block px-4 py-2 hover:bg-gray-100">Hoodies</a>
                            <a href="#" class="block px-4 py-2 hover:bg-gray-100">T-Shirts</a>
                            <a href="#" class="block px-4 py-2 hover:bg-gray-100">Shoes</a>
                        </div>
                    </div>
                    <a href="#" class="hover:text-gray-600">Collections</a>
                    <a href="#" class="hover:text-gray-600">Sale</a>
                </nav>
            </div>
            <div class="flex items-center space-x-6">
                <div class="relative">
                    <i class="fas fa-search cursor-pointer"></i>
                </div>
                <div class="relative">
                    <i class="fas fa-heart cursor-pointer"></i>
                </div>
                <div class="relative">
                    <i class="fas fa-shopping-bag cursor-pointer"></i>
                    <span class="cart-count">0</span>
                </div>
                <div class="hidden md:block">
                    <a href="#" class="px-4 py-2 text-sm">Sign In</a>
                    <a href="#" class="px-4 py-2 bg-black text-white text-sm rounded">Join Us</a>
                </div>
                <button class="md:hidden">
                    <i class="fas fa-bars"></i>
                </button>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero-section flex items-center">
        <div class="container mx-auto px-4 text-white">
            <div class="max-w-2xl">
                <h1 class="text-5xl md:text-7xl font-extrabold mb-4 leading-tight">SHOUPAY SUPREME COLLECTION</h1>
                <p class="text-xl mb-8">Performance engineered for the streets</p>
                <div class="flex space-x-4">
                    <a href="#" class="px-8 py-4 bg-white text-black font-bold rounded-full hover:bg-gray-100 transition-all duration-300 transform hover:scale-105">Shop Now</a>
                    <a href="#" class="px-8 py-4 border-2 border-white text-white font-bold rounded-full hover:bg-white hover:text-black transition-all">Explore</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Featured Categories -->
    <section class="py-16">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold mb-12 text-center">Shop by Category</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="relative overflow-hidden group">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/cc9a0888-cf99-4555-ab4a-47563eb4ddc9.png" alt="Assortment of stylish hoodies in various colors displayed on hangers against a dark background" class="w-full h-auto transition duration-500 group-hover:scale-105" />
                    <div class="absolute bottom-0 left-0 right-0 bg-black bg-opacity-70 text-white p-6">
                        <h3 class="text-2xl font-bold mb-2">Hoodies</h3>
                        <a href="#" class="text-sm font-semibold hover:underline">Shop Now <i class="fas fa-arrow-right ml-1"></i></a>
                    </div>
                </div>
                <div class="relative overflow-hidden group">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/b54c6825-3210-4012-af73-5f44b83fb928.png" alt="Minimalist t-shirts folded neatly in pastel colors displayed on a wooden shelf" class="w-full h-auto transition duration-500 group-hover:scale-105" />
                    <div class="absolute bottom-0 left-0 right-0 bg-black bg-opacity-70 text-white p-6">
                        <h3 class="text-2xl font-bold mb-2">T-Shirts</h3>
                        <a href="#" class="text-sm font-semibold hover:underline">Shop Now <i class="fas fa-arrow-right ml-1"></i></a>
                    </div>
                </div>
                <div class="relative overflow-hidden group">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/bdc15059-2175-4ef3-9212-2089c870a774.png" alt="Modern sneakers in a row showing different angles and color variations on a white background" class="w-full h-auto transition duration-500 group-hover:scale-105" />
                    <div class="absolute bottom-0 left-0 right-0 bg-black bg-opacity-70 text-white p-6">
                        <h3 class="text-2xl font-bold mb-2">Sneakers</h3>
                        <a href="#" class="text-sm font-semibold hover:underline">Shop Now <i class="fas fa-arrow-right ml-1"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Featured Products -->
    <section class="py-16 bg-gray-100">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold mb-12 text-center">Featured Products</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Product 1 -->
                <div class="product-card bg-white rounded-lg overflow-hidden transition duration-300 group">
                    <div class="relative">
                    <div class="relative overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/65709bcf-19eb-491a-b3d1-ed857b83520d.png" alt="Black oversized hoodie with embroidered logo on chest, model wearing it with jeans" class="w-full" />
                        <div class="absolute top-0 left-0 bg-black text-white px-3 py-1 text-xs font-bold">NEW</div>
                        <div class="absolute top-0 right-0 flex flex-col space-y-2 p-2">
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-heart"></i>
                            </button>
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200 product-actions" onclick="showQuickView('product1')">
                                <i class="fas fa-expand"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold mb-1">Oversized Logo Hoodie</h3>
                        <p class="text-gray-500 text-sm mb-2">Men's Streetwear</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold">$89.99</span>
                            <div class="flex space-x-1">
                                <div class="w-4 h-4 rounded-full bg-black"></div>
                                <div class="w-4 h-4 rounded-full bg-gray-500 border border-gray-300"></div>
                                <div class="w-4 h-4 rounded-full bg-red-500"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Product 2 -->
                <div class="product-card bg-white rounded-lg overflow-hidden transition duration-300">
                    <div class="relative overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/8eb616de-e479-49f0-a0a6-2bd6e69e8b32.png" alt="White basic t-shirt with small logo print on left chest, minimalist design" class="w-full" />
                        <div class="absolute top-0 right-0 flex flex-col space-y-2 p-2">
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-heart"></i>
                            </button>
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-expand"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold mb-1">Essential Logo T-Shirt</h3>
                        <p class="text-gray-500 text-sm mb-2">Men's Basics</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold">$29.99</span>
                            <div class="flex space-x-1">
                                <div class="w-4 h-4 rounded-full bg-white border border-gray-300"></div>
                                <div class="w-4 h-4 rounded-full bg-black"></div>
                                <div class="w-4 h-4 rounded-full bg-navy-blue"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Product 3 -->
                <div class="product-card bg-white rounded-lg overflow-hidden transition duration-300">
                    <div class="relative overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/9035adb7-c4be-4e26-9ba6-c85f7a9894dc.png" alt="Sporty sneakers with breathable mesh and cushioned soles in white and gray colorway" class="w-full" />
                        <div class="absolute top-0 left-0 bg-red-500 text-white px-3 py-1 text-xs font-bold">SALE</div>
                        <div class="absolute top-0 right-0 flex flex-col space-y-2 p-2">
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-heart"></i>
                            </button>
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-expand"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold mb-1">SHOUPAY Motion Sneakers</h3>
                        <p class="text-gray-500 text-sm mb-2">Men's Footwear</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold">$129.99 <span class="text-red-500 line-through ml-2 text-sm">$149.99</span></span>
                            <div class="flex space-x-1">
                                <div class="w-4 h-4 rounded-full bg-white border border-gray-300"></div>
                                <div class="w-4 h-4 rounded-full bg-gray-300"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Product 4 -->
                <div class="product-card bg-white rounded-lg overflow-hidden transition duration-300">
                    <div class="relative overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/b3f7b656-fd6f-4832-b3d0-bc54dc0c0ada.png" alt="Cropped hoodie in light pink with matching sweatpants, modeled on female mannequin" class="w-full" />
                        <div class="absolute top-0 right-0 flex flex-col space-y-2 p-2">
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-heart"></i>
                            </button>
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-expand"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold mb-1">Cropped Hoodie Set</h3>
                        <p class="text-gray-500 text-sm mb-2">Women's Set</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold">$119.99</span>
                            <div class="flex space-x-1">
                                <div class="w-4 h-4 rounded-full bg-pink-200"></div>
                                <div class="w-4 h-4 rounded-full bg-lavender"></div>
                                <div class="w-4 h-4 rounded-full bg-gray-300"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="text-center mt-12">
                <a href="#" class="px-8 py-3 border-2 border-black font-semibold rounded hover:bg-black hover:text-white">View All Products</a>
            </div>
        </div>
    </section>

    <!-- Best Sellers -->
    <section class="py-16">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold mb-12 text-center">Best Sellers</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Product 5 -->
                <div class="product-card bg-white rounded-lg overflow-hidden transition duration-300">
                    <div class="relative overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/3b60067c-eb02-4cae-93b2-832236903807.png" alt="Black hoodie with graphic print of city skyline, model wearing with black jeans" class="w-full" />
                        <div class="absolute top-0 left-0 bg-black text-white px-3 py-1 text-xs font-bold">BEST SELLER</div>
                        <div class="absolute top-0 right-0 flex flex-col space-y-2 p-2">
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-heart"></i>
                            </button>
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-expand"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold mb-1">SHOUPAY Graphic Hoodie</h3>
                        <p class="text-gray-500 text-sm mb-2">Men's Streetwear</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold">$79.99</span>
                            <div class="flex space-x-1">
                                <div class="w-4 h-4 rounded-full bg-black"></div>
                                <div class="w-4 h-4 rounded-full bg-gray-700"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Product 6 -->
                <div class="product-card bg-white rounded-lg overflow-hidden transition duration-300">
                    <div class="relative overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/8c0e3879-f05a-4731-86a5-cc1a84f4367d.png" alt="Structured white sneakers with leather detailing and gum sole, isolated view" class="w-full" />
                        <div class="absolute top-0 left-0 bg-black text-white px-3 py-1 text-xs font-bold">BEST SELLER</div>
                        <div class="absolute top-0 right-0 flex flex-col space-y-2 p-2">
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-heart"></i>
                            </button>
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-expand"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold mb-1">Classic White Sneakers</h3>
                        <p class="text-gray-500 text-sm mb-2">Unisex Footwear</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold">$109.99</span>
                            <div class="flex space-x-1">
                                <div class="w-4 h-4 rounded-full bg-white border border-gray-300"></div>
                                <div class="w-4 h-4 rounded-full bg-black"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Product 7 -->
                <div class="product-card bg-white rounded-lg overflow-hidden transition duration-300">
                    <div class="relative overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/4b209c3e-96ac-4c36-8643-2d4a3c78e336.png" alt="Oversized black t-shirt with bold white typography print, streetwear style" class="w-full" />
                        <div class="absolute top-0 left-0 bg-black text-white px-3 py-1 text-xs font-bold">BEST SELLER</div>
                        <div class="absolute top-0 right-0 flex flex-col space-y-2 p-2">
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-heart"></i>
                            </button>
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-expand"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold mb-1">Oversized Print T-Shirt</h3>
                        <p class="text-gray-500 text-sm mb-2">Unisex Streetwear</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold">$39.99</span>
                            <div class="flex space-x-1">
                                <div class="w-4 h-4 rounded-full bg-black"></div>
                                <div class="w-4 h-4 rounded-full bg-white border border-gray-300"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Product 8 -->
                <div class="product-card bg-white rounded-lg overflow-hidden transition duration-300">
                    <div class="relative overflow-hidden">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/daba86c2-463c-4b78-b9b5-27d3f7d3a8d6.png" alt="High-top sneakers in black and red colorway with unique strap details" class="w-full" />
                        <div class="absolute top-0 left-0 bg-black text-white px-3 py-1 text-xs font-bold">BEST SELLER</div>
                        <div class="absolute top-0 right-0 flex flex-col space-y-2 p-2">
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-heart"></i>
                            </button>
                            <button class="bg-white p-2 rounded-full hover:bg-gray-200">
                                <i class="fas fa-expand"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="font-semibold mb-1">High-Top Street Sneakers</h3>
                        <p class="text-gray-500 text-sm mb-2">Men's Footwear</p>
                        <div class="flex justify-between items-center">
                            <span class="font-bold">$139.99</span>
                            <div class="flex space-x-1">
                                <div class="w-4 h-4 rounded-full bg-black"></div>
                                <div class="w-4 h-4 rounded-full bg-red-500"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Special Offer -->
    <section class="py-16 bg-black text-white">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <div>
                    <h2 class="text-4xl font-bold mb-4">LIMITED TIME OFFER</h2>
                    <p class="text-xl mb-6">20% OFF YOUR FIRST ORDER</p>
                    <p class="mb-8">Sign up for our newsletter and get an exclusive discount on your first purchase. Stay updated with our latest collections and special offers.</p>
                    <form class="flex flex-col sm:flex-row gap-3">
                        <input type="email" placeholder="Your email address" class="px-4 py-3 w-full sm:w-96 bg-gray-800 text-white placeholder-gray-400 rounded" />
                        <button type="submit" class="px-6 py-3 bg-white text-black font-semibold rounded hover:bg-gray-200">SUBSCRIBE</button>
                    </form>
                </div>
                <div class="relative">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/dddd4df7-8545-42fe-ad12-f6bc446fbccd.png" alt="Stylish model wearing brand's signature hoodie and sneakers in an SHOUPAY setting at golden hour" class="w-full rounded-lg" />
                    <div class="absolute -bottom-6 -right-6 bg-white text-black px-6 py-3 rounded-lg shadow-lg">
                        <span class="font-bold text-xl">20% OFF</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Product Spotlight -->
    <section class="py-16">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <div class="grid grid-cols-2 gap-4">
                    <div class="relative overflow-hidden rounded-lg">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/95528a0d-4560-4714-9e59-f57d2ad3fb8f.png" alt="Close-up of premium fabric texture showing stitching details of the hoodie" class="w-full h-full object-cover" />
                    </div>
                    <div class="relative overflow-hidden rounded-lg row-span-2">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/67f42afa-4b52-4805-93a1-ecb2f75a060f.png" alt="Full body shot of model wearing the featured hoodie with matching joggers in street style" class="w-full h-full object-cover" />
                    </div>
                    <div class="relative overflow-hidden rounded-lg">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/22195760-99c1-461b-9d7e-bac6083e9d69.png" alt="Detail shot of the embroidered brand logo on the chest area of the hoodie" class="w-full h-full object-cover" />
                    </div>
                </div>
                <div>
                    <h2 class="text-4xl font-bold mb-4">PREMIUM ESSENTIAL HOODIE</h2>
                    <p class="text-xl text-gray-600 mb-6">Crafted for comfort and style</p>
                    <div class="mb-6">
                        <span class="text-red-500 font-bold text-2xl">$89.99</span>
                        <span class="text-gray-400 line-through ml-2">$99.99</span>
                    </div>
                    <p class="mb-6">Our signature hoodie features premium cotton blend fabric, reinforced stitching, and a relaxed fit designed for all-day comfort. The adjustable drawstring hood and kangaroo pocket provide both style and functionality.</p>
                    
                    <div class="mb-8">
                        <h3 class="font-bold mb-3">COLOR: <span class="font-normal">Black</span></h3>
                        <div class="flex space-x-2">
                            <div class="w-8 h-8 rounded-full bg-black border-2 border-black"></div>
                            <div class="w-8 h-8 rounded-full bg-gray-500 border-2 border-gray-300"></div>
                            <div class="w-8 h-8 rounded-full bg-navy-blue border-2 border-gray-300"></div>
                        </div>
                    </div>
                    
                    <div class="mb-8">
                        <h3 class="font-bold mb-3">SIZE:</h3>
                        <div class="size-selector grid grid-cols-5 gap-2 max-w-sm">
                            <input type="radio" name="size" id="size-xs" class="hidden" />
                            <label for="size-xs" class="border border-gray-300 rounded py-2 text-center cursor-pointer hover:border-black">XS</label>
                            <input type="radio" name="size" id="size-s" class="hidden" />
                            <label for="size-s" class="border border-gray-300 rounded py-2 text-center cursor-pointer hover:border-black">S</label>
                            <input type="radio" name="size" id="size-m" class="hidden" checked />
                            <label for="size-m" class="border border-gray-300 rounded py-2 text-center cursor-pointer hover:border-black">M</label>
                            <input type="radio" name="size" id="size-l" class="hidden" />
                            <label for="size-l" class="border border-gray-300 rounded py-2 text-center cursor-pointer hover:border-black">L</label>
                            <input type="radio" name="size" id="size-xl" class="hidden" />
                            <label for="size-xl" class="border border-gray-300 rounded py-2 text-center cursor-pointer hover:border-black">XL</label>
                        </div>
                    </div>
                    
                    <button class="w-full bg-black text-white py-4 rounded font-semibold mb-4 hover:bg-gray-800">
                        ADD TO CART — $89.99
                    </button>
                    
                    <div class="flex items-center space-x-4 text-sm text-gray-600">
                        <div class="flex items-center">
                            <i class="fas fa-shipping-fast mr-2"></i>
                            <span>Free shipping</span>
                        </div>
                        <div class="flex items-center">
                            <i class="fas fa-exchange-alt mr-2"></i>
                            <span>Free returns</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="py-16 bg-gray-100">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold mb-12 text-center">What Our Customers Say</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-white rounded-lg shadow-sm p-8">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                        <span class="text-sm text-gray-500">5/5</span>
                    </div>
                    <p class="text-gray-700 mb-6">"The quality of the hoodie exceeded my expectations. The fabric is so soft and comfortable. Will definitely be buying more colors!"</p>
                    <div class="flex items-center">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/5b67e883-cae0-48c3-9376-76ce60467b95.png" alt="Portrait of satisfied female customer with short blonde hair and blue eyes" class="w-full h-full object-cover" />
                        </div>
                        <div>
                            <p class="font-semibold">Sarah J.</p>
                            <p class="text-sm text-gray-500">Verified Customer</p>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-sm p-8">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                        <span class="text-sm text-gray-500">5/5</span>
                    </div>
                    <p class="text-gray-700 mb-6">"Best sneakers I've ever owned! They're comfortable enough to wear all day and stylish enough for any occasion. Worth every penny."</p>
                    <div class="flex items-center">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/0c2a7b38-af1e-4453-ab20-c651445aed6f.png" alt="Portrait of happy male customer with beard wearing a cap" class="w-full h-full object-cover" />
                        </div>
                        <div>
                            <p class="font-semibold">Michael T.</p>
                            <p class="text-sm text-gray-500">Verified Customer</p>
                        </div>
                    </div>
                </div>
                
                <div class="bg-white rounded-lg shadow-sm p-8">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star-half-alt"></i>
                        </div>
                        <span class="text-sm text-gray-500">4.5/5</span>
                    </div>
                    <p class="text-gray-700 mb-6">"The t-shirt collection is amazing. Perfect fit, great quality fabric, and the colors don't fade even after multiple washes."</p>
                    <div class="flex items-center">
                        <div class="w-12 h-12 rounded-full overflow-hidden mr-4">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/f5d20385-9aae-4fda-86e7-0dcd5e7cfd6a.png" alt="Portrait of young female customer with curly hair smiling brightly" class="w-full h-full object-cover" />
                        </div>
                        <div>
                            <p class="font-semibold">Alexandra P.</p>
                            <p class="text-sm text-gray-500">Verified Customer</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black text-white pt-16 pb-8">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12">
                <div>
                    <h3 class="text-xl font-bold mb-6">IKHO</h3>
                    <p class="text-gray-400 mb-6">Premium streetwear fashion for the SHOUPAY lifestyle.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-facebook"></i></a>
                        <a href="#" class="text-gray-400 hover:text-white"><i class="fab fa-pinterest"></i></a>
                    </div>
                </div>
                <div>
                    <h4 class="font-bold text-lg mb-6">SHOP</h4>
                    <ul class="space-y-3">
                        <li><a href="#" class="text-gray-400 hover:text-white">Men's Collection</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Women's Collection</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">New Arrivals</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Best Sellers</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Sale Items</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold text-lg mb-6">HELP</h4>
                    <ul class="space-y-3">
                        <li><a href="#" class="text-gray-400 hover:text-white">Customer Service</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Track Order</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Returns & Exchanges</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">Shipping Information</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white">FAQ</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-bold text-lg mb-6">CONTACT</h4>
                    <ul class="space-y-3 text-gray-400">
                        <li class="flex items-start">
                            <i class="fas fa-map-marker-alt mt-1 mr-3"></i>
                            <span>123 Fashion Street, Los Angeles, CA 90015</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-phone-alt mr-3"></i>
                            <span>+1 (800) 123-4567</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-envelope mr-3"></i>
                            <span>info@SHOUPAY.com</span>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-500 text-sm mb-4 md:mb-0">© 2023 SHOUPAY. All rights reserved.</p>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-500 hover:text-white text-sm">Privacy Policy</a>
                    <a href="#" class="text-gray-500 hover:text-white text-sm">Terms of Service</a>
                    <a href="#" class="text-gray-500 hover:text-white text-sm">Accessibility</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Quick View Modal -->
    <div id="quickViewModal" class="fixed inset-0 bg-black bg-opacity-50 z-50 hidden flex items-center justify-center p-4">
        <div class="bg-white rounded-lg max-w-4xl w-full max-h-[90vh] overflow-y-auto">
            <div class="p-6">
                <div class="flex justify-between items-start mb-6">
                    <h3 class="text-2xl font-bold">QUICK VIEW</h3>
                    <button onclick="hideQuickView()" class="text-2xl">&times;</button>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                    <div class="space-y-4">
                        <img id="quickViewImage" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/98fec049-76bd-4d8a-b700-0b6ae1a8a3b8.png" alt="Product image" class="w-full rounded-lg">
                        <div class="grid grid-cols-4 gap-2">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/91c08450-6ab3-408a-9132-3b720bb2e7a9.png" alt="Thumbnail" class="cursor-pointer border rounded hover:border-black">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/ff179a0d-1a2a-4672-90ec-98f7b7e71059.png" alt="Thumbnail" class="cursor-pointer border rounded hover:border-black">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/9bf402d4-465d-4500-90d1-6a9b36062c0e.png" alt="Thumbnail" class="cursor-pointer border rounded hover:border-black">
                            <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/15095b55-ee6b-4f8e-aa00-6e5b841c08c5.png" alt="Thumbnail" class="cursor-pointer border rounded hover:border-black">
                        </div>
                    </div>
                    <div>
                        <h2 id="quickViewTitle" class="text-3xl font-bold mb-2">Product Name</h2>
                        <p id="quickViewPrice" class="text-2xl mb-4">$129.99</p>
                        <div class="mb-6">
                            <div class="flex items-center mb-2">
                                <div class="text-yellow-400 mr-2">
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star-half-alt"></i>
                                </div>
                                <span class="text-sm">(42 Reviews)</span>
                            </div>
                            <p class="text-gray-600 mb-4">Premium quality fabric with attention to detail that makes all the difference for performance and comfort.</p>
                        </div>
                        <!-- Size and color selectors would go here -->
                        <button class="w-full bg-black text-white py-4 rounded font-semibold mb-4 hover:bg-gray-800">ADD TO CART</button>
                        <div class="flex items-center space-x-4 text-sm text-gray-600">
                            <div class="flex items-center">
                                <i class="fas fa-shipping-fast mr-2"></i>
                                <span>Free shipping</span>
                            </div>
                            <div class="flex items-center">
                                <i class="fas fa-exchange-alt mr-2"></i>
                                <span>Free returns</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Quick View Functions
        function showQuickView(productId) {
            // In a real implementation, you'd fetch product data based on the ID
            document.getElementById('quickViewModal').classList.remove('hidden');
            document.body.classList.add('overflow-hidden');
        }
        
        function hideQuickView() {
            document.getElementById('quickViewModal').classList.add('hidden');
            document.body.classList.remove('overflow-hidden');
        }
        // Shopping cart functionality
        let cartCount = 0;
        const cartButtons = document.querySelectorAll('.product-card button:not(.fa-heart)');
        const cartIcon = document.querySelector('.fa-shopping-bag');
        const cartNumber = document.querySelector('.cart-count');
        
        cartButtons.forEach(button => {
            button.addEventListener('click', (e) => {
                if (e.currentTarget.classList.contains('fa-heart')) return;
                
                cartCount++;
                cartNumber.textContent = cartCount;
                
                // Animation for cart icon
                cartIcon.parentElement.classList.add('animate-bounce');
                setTimeout(() => {
                    cartIcon.parentElement.classList.remove('animate-bounce');
                }, 1000);
                
                // Notification
                alert('Item added to cart!');
            });
        });
        
        // Mobile menu toggle (would need actual mobile menu HTML)
        const mobileMenuButton = document.querySelector('.md\\:hidden');
        mobileMenuButton.addEventListener('click', () => {
            alert('Mobile menu would open here');
        });
    </script>
</body>
</html>


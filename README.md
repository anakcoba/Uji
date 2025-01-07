<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PT. CIP Energi - Geothermal & Oilfield Equipment</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/tailwindcss/2.2.19/tailwind.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/alpinejs" defer></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Poppins:wght@400;600;700&display=swap');
        body {
            font-family: 'Poppins', sans-serif;
        }
        .clip-shape {
            clip-path: polygon(0 0, 100% 0, 100% 60%, 0 80%);
        }
    </style>
</head>
<body class="bg-gray-50" x-data="{ open: false }">
    <!-- Navigation -->
    <nav class="bg-blue-900 text-white shadow-lg fixed w-full z-50">
        <div class="container mx-auto px-4 py-4 flex justify-between items-center">
            <h1 class="text-2xl font-bold">PT. CIP Energi</h1>
            <div class="hidden md:flex space-x-6">
                <a href="#home" class="hover:text-blue-200">Home</a>
                <a href="#about" class="hover:text-blue-200">About</a>
                <a href="#products" class="hover:text-blue-200">Products</a>
                <a href="#contact" class="hover:text-blue-200">Contact</a>
            </div>
            <button @click="open = !open" class="md:hidden focus:outline-none" aria-label="Toggle Menu">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                </svg>
            </button>
        </div>
        <div x-show="open" class="md:hidden bg-blue-800 text-white">
            <a href="#home" class="block px-4 py-2 hover:bg-blue-700">Home</a>
            <a href="#about" class="block px-4 py-2 hover:bg-blue-700">About</a>
            <a href="#products" class="block px-4 py-2 hover:bg-blue-700">Products</a>
            <a href="#contact" class="block px-4 py-2 hover:bg-blue-700">Contact</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <header id="home" class="relative min-h-screen flex items-center pt-16">
        <div class="absolute inset-0 z-0">
            <img src="Background.jpg" alt="Industrial machinery" class="w-full h-full object-cover" />
        </div>
        <div class="absolute inset-0 z-5 bg-gradient-to-br from-blue-900 to-blue-600 opacity-90 clip-shape"></div>
        <div class="container mx-auto px-4 text-center relative z-10">
            <div class="px-8 py-6 max-w-4xl mx-auto">
                <h2 class="text-6xl font-extrabold text-white drop-shadow-lg mb-6 leading-tight">
                    Geothermal & Oilfield Equipment Solutions
                </h2>
                <p class="text-2xl text-white font-light mb-8 drop-shadow-md">
                    Leading provider of high-quality equipment and reliable service since 2010
                </p>
                <a href="#contact" 
                   class="bg-white text-blue-900 px-10 py-4 rounded-full font-semibold hover:bg-blue-100 
                   inline-block transform hover:scale-105 transition-transform duration-300">
                    Get Started
                </a>
            </div>
        </div>
    </header>

    <!-- Remaining Sections -->
    <!-- About, Products, Contact, and Footer sections remain unchanged -->

</body>
</html>

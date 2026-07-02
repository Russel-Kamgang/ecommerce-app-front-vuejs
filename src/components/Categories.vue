<template>
    <section id="categories" class="py-16 scroll-mt-20 bg-white">
        <div class="container mx-auto px-4">
            <!-- Section Header  -->
            <div class="text-center mb-12">
                <h2 class="text-2xl font-bold text-amber-950 mb-3">Explore Our Fragance Collections</h2>
                <p class="text-lg text-gray-800 max-w-2xl mx-auto">Discover scents that match your personality</p>
            </div>

            <!-- Categories Grid  -->
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                <div v-for="(category, index) in categories" :key="index"
                    class="relative group overflow-hidden rounded-lg shadow-md hover:shadow-lg transition-shadow duration-300">
                    <div class="h-64 overflow-hidden">
                        <img :src="category.image" :alt="category.alt"
                            class="w-ful h-full object-cover group-hover:scale-105 transition-transform duration-500">
                    </div>
                    <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent">
                        <div class="absolute bottom-0 left-0 p-6">
                            <h3 class="text-xl font-semibold text-white">{{ category.title }}</h3>
                            <p class="text-gray-200 mt-1">{{ category.description }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';

import productImage from '../assets/product.jpeg';
import product1Image from '../assets/product1.jpeg';
import product2Image from '../assets/product2.png';
import product3Image from '../assets/product3.webp';
import product4Image from '../assets/product4.jpg';
import product5Image from '../assets/product5.jpg';

const categories = ref([
    { image: productImage, title: "Men's Collection", description: "Bold & masculine scents", alt: "Men's Collection" },
    { image: product1Image, title: "Women's Collection", description: "Bold & feminine scents", alt: "women's Collection" },
    { image: product2Image, title: "Men's Collection", description: "Bold & masculine scents", alt: "Men's Collection" },
    { image: product3Image, title: "Men's Collection", description: "Bold & masculine scents", alt: "Men's Collection" },
    { image: product4Image, title: "Men's Collection", description: "Bold & masculine scents", alt: "Men's Collection" },
    { image: product5Image, title: "Men's Collection", description: "Bold & masculine scents", alt: "Men's Collection" },
])

</script>
<template>
    <div id="app" class="antialiased text-gray-900">
        <!-- <div class="bg-gray-800 min-h-screen py-32 px-6">
            <AccountDropdown />
        </div> -->
        <div class="bg-gray-200 min-h-screen">
            <Navbar />
        </div>
        <!-- <div
            class="bg-gray-200 min-h-screen p-8 flex items-center justify-center"
        >
            <PropertyCard :property="property" />
        </div> -->
    </div>
</template>

<script>
import Navbar from './components/Navbar'
// import PropertyCard from './components/PropertyCard.vue'
// import AccountDropdown from './components/AccountDropdown'

export default {
    name: 'App',
    components: {
        // AccountDropdown
        Navbar
        // PropertyCard
    },
    data() {
        return {
            property: {
                imageUrl:
                    'https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80',
                imageAlt: 'Rear view of modern home with pool',
                beds: 3,
                baths: 2,
                title: 'Modern home in city center',
                // title: 'Modern executive home in the heart of hitoric Los Angeles',
                priceInCents: 190000,
                formattedPrice: '$1,900.00',
                reviewCount: 34,
                rating: 4
            }
        }
    }
}
</script>

<style src="./assets/tailwind.css"></style>

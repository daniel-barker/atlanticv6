<script lang="ts">
  const valueProps = [
    {
      icon: 'quality',
      title: 'Premium Quality',
      description: 'Top-grade materials and expert craftsmanship for lasting durability'
    },
    {
      icon: 'delivery',
      title: 'Fast Delivery',
      description: 'Efficient delivery service to meet your project timeline'
    },
    {
      icon: 'support',
      title: 'Expert Support',
      description: '40+ years of experience in gutter solutions'
    }
  ];

  const featuredProducts = [
    {
      image: '/images/products/k-style.jpg',
      title: 'K-Style Gutters',
      description: 'Our most popular gutter style, perfect for modern homes'
    },
    {
      image: '/images/products/half-round.jpg',
      title: 'Half Round Gutters',
      description: 'Classic design ideal for historic and traditional architecture'
    },
    {
      image: '/images/products/euro.jpg',
      title: 'Euro Gutters',
      description: 'European-inspired design for contemporary aesthetics'
    }
  ];
</script>

<!-- Hero Section -->
<section class="relative bg-gray-900 text-white">
  <div class="absolute inset-0 bg-black/50"></div>
  <div
    class="relative container mx-auto px-4 py-24 flex flex-col items-center text-center"
    style="background-image: url('/images/hero-bg.jpg'); background-size: cover; background-position: center;"
  >
    <h1 class="text-4xl md:text-6xl font-bold mb-6">
      Quality Gutter Solutions for Every Project
    </h1>
    <p class="text-xl md:text-2xl mb-8 max-w-2xl">
      Your trusted source for professional gutter supplies and expert consultation
    </p>
    <div class="flex gap-4">
      <a
        href="/products"
        class="bg-blue-600 hover:bg-blue-700 text-white px-8 py-3 rounded-lg font-medium transition-colors"
      >
        View Products
      </a>
      <a
        href="/contact"
        class="bg-white hover:bg-gray-100 text-gray-900 px-8 py-3 rounded-lg font-medium transition-colors"
      >
        Contact Us
      </a>
    </div>
  </div>
</section>

<!-- Value Propositions -->
<section class="py-16 bg-gray-50">
  <div class="container mx-auto px-4">
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      {#each valueProps as prop}
        <div class="text-center p-6 bg-white rounded-lg shadow-sm">
          <div class="w-16 h-16 mx-auto mb-4 bg-blue-100 rounded-full flex items-center justify-center">
            <!-- Placeholder for icon -->
            <div class="w-8 h-8 bg-blue-600 rounded-full"></div>
          </div>
          <h3 class="text-xl font-semibold mb-2">{prop.title}</h3>
          <p class="text-gray-600">{prop.description}</p>
        </div>
      {/each}
    </div>
  </div>
</section>

<!-- About Preview -->
<section class="py-16">
  <div class="container mx-auto px-4">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
      <div>
        <h2 class="text-3xl font-bold mb-6">Your Trusted Partner Since [YEAR]</h2>
        <p class="text-gray-600 mb-6">
          Atlantic Gutter Supply has been serving contractors and homeowners with premium
          gutter solutions for over four decades. Our commitment to quality and customer
          service has made us the go-to supplier in the region.
        </p>
        <a
          href="/about"
          class="inline-flex items-center text-blue-600 hover:text-blue-700 font-medium"
        >
          Learn More
          <svg
            class="w-5 h-5 ml-2"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M9 5l7 7-7 7"
            />
          </svg>
        </a>
      </div>
      <div class="relative h-[400px] bg-gray-200 rounded-lg">
        <!-- Placeholder for about image -->
        <div class="absolute inset-0 flex items-center justify-center text-gray-400">
          [About Image Placeholder]
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Featured Products -->
<section class="py-16 bg-gray-50">
  <div class="container mx-auto px-4">
    <h2 class="text-3xl font-bold text-center mb-12">Featured Products</h2>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      {#each featuredProducts as product}
        <div class="bg-white rounded-lg overflow-hidden shadow-sm">
          <div class="relative h-48 bg-gray-200">
            <!-- Placeholder for product image -->
            <div class="absolute inset-0 flex items-center justify-center text-gray-400">
              [Product Image Placeholder]
            </div>
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold mb-2">{product.title}</h3>
            <p class="text-gray-600 mb-4">{product.description}</p>
            <a
              href="/products"
              class="text-blue-600 hover:text-blue-700 font-medium inline-flex items-center"
            >
              View Details
              <svg
                class="w-5 h-5 ml-2"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M9 5l7 7-7 7"
                />
              </svg>
            </a>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>

<!-- Knowledge Base Teaser -->
<section class="py-16 bg-blue-600 text-white">
  <div class="container mx-auto px-4 text-center">
    <h2 class="text-3xl font-bold mb-6">Expert Knowledge at Your Fingertips</h2>
    <p class="text-xl mb-8 max-w-2xl mx-auto">
      Explore our comprehensive guides and resources to make informed decisions about your
      gutter systems.
    </p>
    <a
      href="/knowledge-base"
      class="inline-block bg-white text-blue-600 px-8 py-3 rounded-lg font-medium hover:bg-gray-100 transition-colors"
    >
      Visit Knowledge Base
    </a>
  </div>
</section>

<script lang="ts">
  import '../app.css';

  const navItems = [
    { href: '/', label: 'Home' },
    { href: '/products', label: 'Products' },
    { href: '/services', label: 'Services' },
    { href: '/about', label: 'About' },
    { href: '/contact', label: 'Contact' }
  ];
</script>

<div class="min-h-screen flex flex-col">
  <header class="bg-white shadow-md">
    <nav class="container mx-auto px-4 py-4">
      <div class="flex justify-between items-center">
        <a href="/" class="flex items-center space-x-2">
          <img src="/images/logo.png" alt="Atlantic Gutter Supply" class="h-12 w-auto" />
        </a>
        
        <div class="hidden md:flex space-x-8">
          {#each navItems as { href, label }}
            <a
              {href}
              class="text-gray-700 hover:text-blue-600 font-medium transition-colors"
            >
              {label}
            </a>
          {/each}
        </div>

        <button
          class="md:hidden p-2"
          aria-label="Menu"
        >
          <svg
            class="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            />
          </svg>
        </button>
      </div>
    </nav>
  </header>

  <main class="flex-1">
    <slot />
  </main>

  <footer class="bg-gray-900 text-white">
    <div class="container mx-auto px-4 py-12">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
        <div>
          <h3 class="text-lg font-semibold mb-4">Atlantic Gutter Supply</h3>
          <p class="text-gray-400">Your trusted partner in gutter solutions since [YEAR]</p>
        </div>
        
        <div>
          <h3 class="text-lg font-semibold mb-4">Quick Links</h3>
          <ul class="space-y-2">
            {#each navItems as { href, label }}
              <li>
                <a
                  {href}
                  class="text-gray-400 hover:text-white transition-colors"
                >
                  {label}
                </a>
              </li>
            {/each}
          </ul>
        </div>

        <div>
          <h3 class="text-lg font-semibold mb-4">Contact</h3>
          <ul class="space-y-2 text-gray-400">
            <li>123 Gutter Lane</li>
            <li>Anytown, ST 12345</li>
            <li>Phone: (555) 123-4567</li>
            <li>Email: info@atlanticgutter.com</li>
          </ul>
        </div>

        <div>
          <h3 class="text-lg font-semibold mb-4">Business Hours</h3>
          <ul class="space-y-2 text-gray-400">
            <li>Monday - Friday: 8am - 6pm</li>
            <li>Saturday: 9am - 2pm</li>
            <li>Sunday: Closed</li>
          </ul>
        </div>
      </div>

      <div class="mt-8 pt-8 border-t border-gray-800 text-center text-gray-400">
        <p>&copy; {new Date().getFullYear()} Atlantic Gutter Supply. All rights reserved.</p>
      </div>
    </div>
  </footer>
</div>

 <script>
      let showMenu = false;
    
      function toggleNavbar() {
        showMenu = !showMenu;
      }
    </script>
    
    <div class= "bg-black">
      <div>
        <nav
          class="container px-6 py-8 mx-auto md:flex md:justify-between md:items-center"
        >
          <div class="flex items-center justify-between">
            <a href="/" class="flex items-center">
                  <img src="/IDLOGO.png" class="h-14 hover:scale-105 duration-200" alt="" />
                  <span class="text-2xl font-semibold whitespace-nowrap dark:text-white"></span>
                </a>
            <!-- Mobile menu button -->
            <div on:click={toggleNavbar} class="flex md:hidden">
              <button
                type="button"
                class="text-white hover:text-gray-400 focus:outline-none focus:text-gray-400"
              >
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
              </svg>
              </button>
            </div>
          </div>
    
          <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
          <div
            class="flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0 {showMenu
              ? 'flex'
              : 'hidden'}"
          >
            <a class="text-white hover:scale-105 duration-200 hover:text-orange-400" href="/home">About</a>
            <a class="text-white hover:scale-105 duration-200 hover:text-orange-400" href="/blog">Services</a>
            <a class="text-white hover:scale-105 duration-200 hover:text-orange-400" href="/contact">Blog</a>
            <a class="text-white hover:scale-105 duration-200 hover:text-orange-400" href="/about">Contact Us</a>
          </div>
        </nav>
      </div>
    </div>
    
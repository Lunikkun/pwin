<template>
  <nav class="bg-[#1782C5] shadow-xl">
    <div class="container mx-auto px-4 py-2 flex justify-between items-center">
      <!-- Logo -->
      <div class="flex items-center">
        <img src="/logo-prowin-international.svg" alt="Prowin Logo" class="h-12 w-auto" />
      </div>
      <!-- Menu Button for Small and Medium Screens -->
      <button class="sm:block md:block lg:hidden text-white focus:outline-none" @click="toggleMenu">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16m-7 6h7"
          />
        </svg>
      </button>

      <!-- Social Icons and Contact Info for Large Screens -->
      <div class="hidden lg:flex space-x-4 justify-center items-center">
        <!-- Social Icons -->
        <a href="#" class="text-white hover:text-gray-200">
          <img src="/public/tiktok-outline-svgrepo-com.svg" width="32" height="32" />
          <span class="sr-only">TikTok Placeholder</span>
        </a>
        <a href="#" class="text-white hover:text-gray-200">
          <img src="/public/instagram-svgrepo-com.svg" width="32" height="32" />
          <span class="sr-only">Instagram Placeholder</span>
        </a>
        <a href="#" class="text-white hover:text-gray-200">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6"
            fill="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              d="M22.675 0h-21.35c-.733 0-1.325.592-1.325 1.325v21.351c0 .733.592 1.324 1.325 1.324h11.495v-9.294h-3.128v-3.622h3.128v-2.671c0-3.1 1.893-4.788 4.659-4.788 1.325 0 2.464.099 2.795.143v3.24h-1.918c-1.504 0-1.796.715-1.796 1.763v2.313h3.591l-.467 3.622h-3.124v9.294h6.127c.733 0 1.325-.591 1.325-1.324v-21.35c0-.733-.592-1.325-1.325-1.325z"
            />
          </svg>
          <span class="sr-only">Facebook Placeholder</span>
        </a>

        <!-- Contact Info -->
        <div class="text-white text-sm flex items-center space-x-4">
          
          <div class="flex items-center justify-center space-x-2">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5"
              fill="currentColor"
              viewBox="0 0 24 24"
            >
            
              <path
                d="M22.54 16.88l-5.27-2.27a1.15 1.15 0 0 0-1.34.33l-2.23 2.73a16.06 16.06 0 0 1-7.73-7.73l2.73-2.23a1.15 1.15 0 0 0 .33-1.34L7.12 1.46A1.15 1.15 0 0 0 5.88.88H2.15A1.15 1.15 0 0 0 1 2.03 19.85 19.85 0 0 0 21.97 23a1.15 1.15 0 0 0 1.15-1.15v-3.73a1.15 1.15 0 0 0-.58-1.24z"
              />
              
            </svg>
            <span class="text-white text-xl">Lina:</span>
            <span class="text-sm">+39 3332221110</span>
          </div>
        </div>
      </div>
    </div>

    <!-- Dropdown Menu for Small and Medium Screens -->
    <div
      v-if="isMenuOpen"
      class="sm:block md:block lg:hidden bg-[#1782C5] text-white p-4 space-y-4"
    >
      <!-- Social Icons -->
      <div class="flex space-x-4 justify-center items-center">
        <a href="#" class="hover:text-gray-200">
          <img src="/public/tiktok-outline-svgrepo-com.svg" width="32" height="32"/>
          <span class="sr-only">TikTok Placeholder</span>
        </a>
        <a href="#" class="hover:text-gray-200">
          <img src="/public/instagram-svgrepo-com.svg" width="32" height="32" />
          <span class="sr-only">Instagram Placeholder</span>
        </a>
        <a href="#" class="hover:text-gray-200">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6"
            fill="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              d="M22.675 0h-21.35c-.733 0-1.325.592-1.325 1.325v21.351c0 .733.592 1.324 1.325 1.324h11.495v-9.294h-3.128v-3.622h3.128v-2.671c0-3.1 1.893-4.788 4.659-4.788 1.325 0 2.464.099 2.795.143v3.24h-1.918c-1.504 0-1.796.715-1.796 1.763v2.313h3.591l-.467 3.622h-3.124v9.294h6.127c.733 0 1.325-.591 1.325-1.324v-21.35c0-.733-.592-1.325-1.325-1.325z"
            />
          </svg>
          <span class="sr-only">Facebook Placeholder</span>
        </a>
      </div>

      <!-- Contact Info -->
      <div class="text-sm flex flex-col items-center space-y-2">
        <span class="text-white text-xl">Lina:</span>
        <div class="flex items-center space-x-2">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-5 w-5"
            fill="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              d="M22.54 16.88l-5.27-2.27a1.15 1.15 0 0 0-1.34.33l-2.23 2.73a16.06 16.06 0 0 1-7.73-7.73l2.73-2.23a1.15 1.15 0 0 0 .33-1.34L7.12 1.46A1.15 1.15 0 0 0 5.88.88H2.15A1.15 1.15 0 0 0 1 2.03 19.85 19.85 0 0 0 21.97 23a1.15 1.15 0 0 0 1.15-1.15v-3.73a1.15 1.15 0 0 0-.58-1.24z"
            />
          </svg>
          <span class="text-sm">+39 3332221110</span>
        </div>
      </div>
    </div>
  </nav>
</template>

<script lang="ts">
export default {
  name: "SiteNavbar",
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>
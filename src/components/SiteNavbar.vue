<template>
  <nav class="bg-[#1782C5] shadow-md">
    <div class="container mx-auto px-4 py-2 flex justify-between items-center">
      <!-- Logo -->
      <div class="flex items-center">
        <img src="/logo-prowin-international.svg" alt="Prowin Logo" class="h-12 w-auto" />
      </div>

      <!-- Social Icons -->
      <div class="flex space-x-4">
        <a href="#" class="text-white hover:text-gray-200">
          <!-- TikTok Icon -->
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6"
            fill="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              d="M9 2v10.5a3.5 3.5 0 1 1-3.5-3.5H7a5 5 0 1 0 5 5V7.1a6.5 6.5 0 0 0 4 1.4V5.6a4.5 4.5 0 0 1-4-1.6V2H9z"
            />
          </svg>
          <span class="sr-only">TikTok Placeholder</span>
        </a>
        <a href="#" class="text-white hover:text-gray-200">
          <!-- Instagram Icon -->
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="h-6 w-6"
            fill="currentColor"
            viewBox="0 0 24 24"
          >
            <path
              d="M12 2.163c3.204 0 3.584.012 4.85.07 1.366.062 2.633.334 3.608 1.308.975.975 1.246 2.242 1.308 3.608.058 1.266.07 1.646.07 4.85s-.012 3.584-.07 4.85c-.062 1.366-.334 2.633-1.308 3.608-.975.975-2.242 1.246-3.608 1.308-1.266.058-1.646.07-4.85.07s-3.584-.012-4.85-.07c-1.366-.062-2.633-.334-3.608-1.308-.975-.975-1.246-2.242-1.308-3.608-.058-1.266-.07-1.646-.07-4.85s.012-3.584.07-4.85c.062-1.366.334-2.633 1.308-3.608.975-.975 2.242-1.246 3.608-1.308 1.266-.058 1.646-.07 4.85-.07zm0-2.163c-3.259 0-3.667.012-4.947.07-1.281.059-2.563.334-3.637 1.408-1.074 1.074-1.349 2.356-1.408 3.637-.058 1.28-.07 1.688-.07 4.947s.012 3.667.07 4.947c.059 1.281.334 2.563 1.408 3.637 1.074 1.074 2.356 1.349 3.637 1.408 1.28.058 1.688.07 4.947.07s3.667-.012 4.947-.07c1.281-.059 2.563-.334 3.637-1.408 1.074-1.074 1.349-2.356 1.408-3.637.058-1.28.07-1.688.07-4.947s-.012-3.667-.07-4.947c-.059-1.281-.334-2.563-1.408-3.637-1.074-1.074-2.356-1.349-3.637-1.408-1.28-.058-1.688-.07-4.947-.07z"
            />
          </svg>
          <span class="sr-only">Instagram Placeholder</span>
        </a>
        <a href="#" class="text-white hover:text-gray-200">
          <!-- Facebook Icon -->
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
      <div class="text-white text-sm flex items-center space-x-4">
        <span>Contattami qui</span>
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
          <span>+39 3332221110</span>
        </div>
      </div>
    </div>
  </nav>
</template>

<script lang="ts">
export default {
  name: "SiteNavbar",
};
</script>

<style scoped></style>

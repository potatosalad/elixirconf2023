<template>
  <footer v-if="$slidev.nav.currentRoute.meta.section === 1" class="absolute bottom-0 left-0 p-2 text-xs opacity-80">
    1. Distribution Protocol
  </footer>
  <footer v-if="$slidev.nav.currentRoute.meta.section === 2" class="absolute bottom-0 left-0 p-2 text-xs opacity-80">
    2. Erlang Dist Filtering
  </footer>
  <footer v-if="$slidev.nav.currentRoute.meta.section === 3" class="absolute bottom-0 left-0 p-2 text-xs opacity-80">
    3. WhatsApp Runtime System
  </footer>
  <footer
    v-if="$slidev.nav.currentLayout !== 'cover'"
    class="absolute bottom-0 right-0 p-2"
  >
    <span v-if="$slidev.nav.clicks < 100">
      {{ $slidev.nav.currentPage }}.{{ $slidev.nav.clicks }} / {{ $slidev.nav.total }}
    </span>
    <span v-else>
      {{ $slidev.nav.currentPage }}.0 / {{ $slidev.nav.total }}
    </span>
  </footer>
</template>
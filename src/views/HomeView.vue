<script setup>
import TheWelcome from "../components/TheWelcome.vue";

// get platform
const platform = navigator.platform;
</script>

<template>
  <main>
    <!-- <TheWelcome /> -->
    <div
      class="container d-flex justify-content-center align-items-center h-100"
    >
      <div class="card shadow-sm rounded-xl">
        <div class="card-body">
          <div class="row">
            <div class="col-12">
              <h1>Hello World</h1>
            </div>

            <div class="col-12 d-flex align-items-center gap-2">
              <span>Press</span>
              <kbd
                class="kbd bg-white border rounded px-2 py-1 text-secondary-emphasis fw-medium"
              >
                <span class="me-1 small">{{
                  platform === "MacIntel" ? "⌘" : "Ctrl"
                }}</span>
                <span>K</span>
              </kbd>
              <span>to open the command palette</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
main {
  height: 100vh;
}
</style>

<script setup>
  import PokemonCards from './components/PokemonCards.vue';
</script>

<template>
  <main>
    <h1>Hero</h1>
    <Suspense>
      <template #default>
        <PokemonCards />
      </template>
      <template #fallback>
        <div>
          <p>Loading...</p>
        </div>
      </template>
    </Suspense>
  </main>
</template>
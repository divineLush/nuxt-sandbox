<template>
  <div>
    <header>
      <h1>This is a default layout</h1>
    </header>
    <main>
      <Nuxt />
    </main>
  </div>
</template>

<style>
html {
  font-family: monospace;
  font-size: 1.3rem;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

h1 {
  margin: 10px 0;
  color: green;
}

h2 {
  margin: 6px 0;
}
</style>

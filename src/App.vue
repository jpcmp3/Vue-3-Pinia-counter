<template>
  <div class="app">
    <nav>
      <RouterLink to="/">Home</RouterLink> |
      <RouterLink to="/about">About</RouterLink> |
      <RouterLink to="/mypage">My Page</RouterLink> |
    </nav>

    <RouterView />
  </div>
</template>

<style>
.app {
  text-align: center;
}
</style>
<template>
  <div>
    <NavBar />
    <div class="container">
      <Nuxt />
    </div>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar";
export default {};
</script>
<style>
* {
  margin: 0;
}
.container {
  max-width: 1000px;
  margin: 0 auto;
}
</style>

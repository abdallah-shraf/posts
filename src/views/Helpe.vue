<template>
  <div class="helpe">
    <h1>{{ pageName }}</h1>
    <p>{{ pageDesc }}</p>
    
  </div>
</template>
<script>
export default {
  data: function () {
    return {
      pageName: "Helpe Us",
      pageDesc: "This Is About Us Page",
    };
  },
  name: "helpe",
};
</script>

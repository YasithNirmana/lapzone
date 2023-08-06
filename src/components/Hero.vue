<template>
    <div class="hero_container">
      <div class="hero_promotions_container"></div>
      <div v-for="(category, index) in categories" :key="index" :class="['hero_category', 'category_' + (index + 1)]">
        <p>{{ category.name }}</p>
        <p>{{ category.description }}</p>
      </div>
      <div v-for="(brand, index) in brands" :key="index" :class="['hero_band', 'brand_' + (index + 1)]">
        <p>{{ brand.name }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        categories: [
          { name: 'All Laptops', description: 'Best Price' },
          { name: 'Gaming Laptops', description: 'Best Prices' },
          { name: 'Corporate Inquiries' }
        ],
        brands: [
          { name: 'Dell' },
          { name: 'Acer' },
          { name: 'MSI' },
          { name: 'Asus' }
        ]
      };
    }
  };
  </script>

<style scoped>
.hero_container {
    height: 500px;
    display: grid;
    grid-template-columns: repeat(5, auto);
    grid-template-rows: repeat(3, auto);
}
.hero_promotions_container{
    background-color: red;
    grid-column-start: 1;
    grid-column-end: 5;
    grid-row-start: 1;
    grid-row-end: 3;
}
.hero_category, .hero_band {
    border: 1px solid black;
}
.category_1 {
    grid-column-start: 5;
    grid-column-end: 6;
    grid-row-start: 1;
    grid-row-end: 2;
}
.category_2 {
    grid-column-start: 5;
    grid-column-end: 6;
    grid-row-start: 2;
    grid-row-end: 3;
}
.category_3 {
    grid-column-start: 5;
    grid-column-end: 6;
    grid-row-start: 3;
    grid-row-end: 4;
}
.brand_1{
    grid-column-start: 1;
    grid-column-end: 2;
    grid-row-start: 3;
    grid-row-end: 4;
}
.brand_2{
    grid-column-start: 2;
    grid-column-end: 3;
    grid-row-start: 3;
    grid-row-end: 4;
}
.brand_3{
    grid-column-start: 3;
    grid-column-end: 4;
    grid-row-start: 3;
    grid-row-end: 4;
}
.brand_4{
    grid-column-start: 4;
    grid-column-end: 5;
    grid-row-start: 3;
    grid-row-end: 4;
}
</style>
<template>
  <header class="product-header">
    <ProductsHeader />
  </header>
  <main class="product-main">
    <Products :products="products" @to-parent="toParent" />
  </main>
  <footer class="product-footer">
    <ProductsFooter />
  </footer>
</template>

<script>
import Products from "./views/Products.vue";
import ProductsHeader from "./components/header.vue";
import ProductsFooter from "./components/footer.vue";
import "./main.css";

export default {
  components: { Products, ProductsHeader, ProductsFooter },
  data() {
    return {
      products: [
        {
          image: "/src/assets/product.jpg",
          name: "WEBER RANGLI EMULSIYA",
          description:
            "Shokolad rangidagi wb863 suv emulsiyasi. Yuqori sifatli akril kopolimerdan tayyorlangan. Tashqi va ichki ishlar uchun. Oddiy namlik bo'lgan xonalarda devor va shiftlarni bo'yash uchun mo'ljallangan.",
          price: "250 000 so'm",
        },
        {
          image: "/src/assets/product.jpg",
          name: "WEBER RANGLI EMULSIYA",
          description:
            "Shokolad rangidagi wb863 suv emulsiyasi. Yuqori sifatli akril kopolimerdan tayyorlangan. Tashqi va ichki ishlar uchun. Oddiy namlik bo'lgan xonalarda devor va shiftlarni bo'yash uchun mo'ljallangan.",
          price: "250 000 so'm",
        },
        {
          image: "/src/assets/product.jpg",
          name: "WEBER RANGLI EMULSIYA",
          description:
            "Shokolad rangidagi wb863 suv emulsiyasi. Yuqori sifatli akril kopolimerdan tayyorlangan. Tashqi va ichki ishlar uchun. Oddiy namlik bo'lgan xonalarda devor va shiftlarni bo'yash uchun mo'ljallangan.",
          price: "250 000 so'm",
        },
        {
          image: "/src/assets/product.jpg",
          name: "WEBER RANGLI EMULSIYA",
          description:
            "Shokolad rangidagi wb863 suv emulsiyasi. Yuqori sifatli akril kopolimerdan tayyorlangan. Tashqi va ichki ishlar uchun. Oddiy namlik bo'lgan xonalarda devor va shiftlarni bo'yash uchun mo'ljallangan.",
          price: "250 000 so'm",
        },
        {
          image: "/src/assets/product.jpg",
          name: "WEBER RANGLI EMULSIYA",
          description:
            "Shokolad rangidagi wb863 suv emulsiyasi. Yuqori sifatli akril kopolimerdan tayyorlangan. Tashqi va ichki ishlar uchun. Oddiy namlik bo'lgan xonalarda devor va shiftlarni bo'yash uchun mo'ljallangan.",
          price: "250 000 so'm",
        },
        {
          image: "/src/assets/product.jpg",
          name: "WEBER RANGLI EMULSIYA",
          description:
            "Shokolad rangidagi wb863 suv emulsiyasi. Yuqori sifatli akril kopolimerdan tayyorlangan. Tashqi va ichki ishlar uchun. Oddiy namlik bo'lgan xonalarda devor va shiftlarni bo'yash uchun mo'ljallangan.",
          price: "250 000 so'm",
        },
      ],
    };
  },
  methods: {
    toParent(fromChild) {
      console.log(fromChild);
    },
  },
};
</script>

<style></style>

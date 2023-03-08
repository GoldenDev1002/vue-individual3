<template>
<div id="app">
<header>
<h1>{{sitename}}</h1>
<button @click="showCheckout">{{ this.cart.length }}
Checkout</button>
</header>
<main>
<component :is="currentView"></component>
</main>
</div>
</template>
<script>
import ProductList from "./components/ProductList.vue";
import Checkout from "./components/Checkout.vue";
export default {
name: "App",
data() { return { sitename: "Vue.js Pet Depot",
cart: [],
currentView: ProductList } },
components: { ProductList, Checkout },
methods: { showCheckout() {
if (this.currentView === ProductList) ...
};
</script>
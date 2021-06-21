<template>
  <div class="w-25 p-3 product-container d-flex flex-column">
    <div class="d-flex flex-row justify-content-center">
      <img style="height: 150px" :src="product.img" />
    </div>
    <div>
      <h3>{{ product.title }}</h3>
      <hr />
    </div>
    <div>
      <p>{{ product.description }}</p>
    </div>
    <div>
      <span>{{ product.price }}</span>
      <button class="btn btn-primary btn-sm float-right">Commander</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      product: {
        img: "https://www.journaldugeek.com/content/uploads/2018/07/macbook-air.jpg",
        title: "MacBook",
        description:
          "D'une finesse et d'une légèreté hors du commun, le MacBook Pro est encore plus rapide et plus puissant qu'avant.",
        price: "1500 €",
      },
    };
  },
};
</script>

<style>
.product-container {
  height: 400px;
}
</style>
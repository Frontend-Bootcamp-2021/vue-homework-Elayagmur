<template>
  <div>
    <h2 class="page-header">BREEDS LIST</h2>
    <ListingComponent :data="listings" @selected="alertBox" />
  </div>
</template>

<script>
import { ref, onMounted, onUnmounted, onUpdated } from "vue";

import ListingComponent from "@/components/Listing.vue";
export default {
  components: {
    ListingComponent,
  },
  setup() {
    onMounted(() => console.log("Mount: ✅ Detail Component"));
    onUnmounted(() => console.log("unMount: 👋🏻 Detail Component "));
    onUpdated(() => console.log("Updated: 🔥 Detail Component"));

    let listings = ref([]);
    setTimeout(() => {
      listings.value = [
        { id: 1, name: "Affenpinscher" },
        { id: 2, name: "Bluetick" },
        { id: 3, name: "Otterhound" },
      ];
    }, 3000);

    const alertBox = (select) => alert(`You selected: ${select}`);

    return {
      listings,
      alertBox,
    };
  },
};
</script>

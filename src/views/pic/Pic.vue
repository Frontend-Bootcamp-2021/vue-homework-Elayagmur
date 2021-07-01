<template>
<div class="image">
  <h1 class="image__title">dog photos</h1>
<button @click="img()">Show Image</button></div>
</template>
‏<script>
import {onMounted } from "vue";
export default{
setup(){
  
let imgEl = document.createElement("img");
function img() {
  imgEl.innerHTML = "";
fetch("https://dog.ceo/api/breeds/image/random")
  .then(res =>  res.json())
      .then(img => img.message)
      .then((src) => {
       imgEl.src = src
       document.body.append(imgEl)
  })
}

let button = document.querySelector("button")
button.addEventListener("click", img);
      onMounted(()=>{
          img();
      })
    return {img};
      },
};

</script>

<style lang="scss">
.image {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  justify-content: flex-start;
&__title{
   display: flex;
  flex-direction: column;
  color: blue;

  }

 
}
</style>


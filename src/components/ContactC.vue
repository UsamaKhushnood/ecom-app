<template>
  <div class="main">
    <b-container class="mt-5">
      <div class="row">
        <div class="col-md-6 p-0">
          <div class="bimg"></div>
        </div>
        <div
          class="col-md-6 p-0 d-flex justify-content-center flex-column bg-light"
        >
          <form-f />
        </div>
      </div>
    </b-container>
  </div>
</template>

<script>
import FormF from "./FormF.vue";
export default {
  components: { FormF },
};
</script>

<style scoped>
h2 {
  font-size: 40px;
  color: blue;
  font-weight: 600;
  font-family: sans-serif;
}
p {
  font-family: sans-serif;
  font-size: 24;
}

.bimg {
  background: url("https://picsum.photos/1200/800");
  min-height: 100%;
}
</style>

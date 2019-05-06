<template>
  <div>
    <input v-model="message">倍も高速化しました!
    <div class="hoshi">
      <span class="message">{{ message }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Hoshi',
  data: function() { 
    return { message: "" };
  },
  props: {
    msg: String
  }
}
</script>

<style scoped>
.hoshi {
  margin: auto;
  width: 559px;
  height: 775px;
  background-image: url("../assets/hoshi_bai.jpg");
  background-repeat: no-repeat;
  background-color: tomato;
}

.message {
  position: relative;
  top: 438px;
  left: 30px;
  width: 220px;
  height: 100px;
  color: #553360dd;
  font-size: 74px;
}
</style>

<template>
  <div class="all">
    <div class="button" @click="addNumb">Numbers</div>
    <div class="tablet">Чиселка побольше: {{ numb }}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      numb: 0,
    };
  },
  methods: {
    addNumb() {
      this.numb += 1;
    },
  },
};
</script>

<style>
.all {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.tablet {
  padding: 5px;
  background: red;
  border-radius: 10px;
}
.button {
  padding: 5px;
  background: blue;
  border-radius: 10px;
}
.button:hover {
  display: inline-block;
  font-size: 1rem;
  background: #ffefba;
  border: 1px solid transparent;
  cursor: pointer;
}
</style>

<template>
  <div id="popup" class="popup">
    <div class="popup_body">
      <div class="popup_content">
        <a href="#" class="close">X</a>
        <div class="title">Модальный заголовок</div>
        <div class="text">Модальный текст</div>
      </div>
    </div>
  </div>
  <a href="#popup" class="button">Жми кнопки</a>
</template>

<script>
export default {
  data() {
    return {
      IsPopUpVisible: false,
    };
  },
  methods: {
    ShowPopup() {
      this.IsPopUpVisible = true;
    },
  },
};
</script>

<style>
.popup {
  width: 100%;
  height: 100vh;
  position: fixed;
  background: rgba(0, 0, 0, 0.5);
  top: 0%;
  left: 0%;
  display: none;
}
.popup:target {
  display: block;
}
.popup_body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100ch;
  padding: 30px 10px;
}
.popup_content {
  background-color: aliceblue;
  color: black;
  max-width: 500px;
  padding: 150px;
  position: relative;
}
.popup_title {
  font-size: 40px;
  margin: 0px 0px 15px 0px;
}
.close {
  font-size: 20px;
  right: 10px;
  top: 10px;
  position: absolute;
  color: black;
  text-decoration: none;
}
.button {
  background-color: rgb(27, 198, 228);
  cursor: pointer;
  user-select: none;
}
</style>

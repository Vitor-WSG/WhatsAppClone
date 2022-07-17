<template>
  <div class="empty">
    <div
      class="
        container
        full-width full-height
        column
        items-center
        justify-center
      "
    >
      <q-img src="../../assets/conect.png" height="250px" width="250px"></q-img>
      <h4>Matenha o Celular Conectado</h4>
      <span>
        O Whatsapp conecta ao seu telefone para sincronizar suas mensagens. Para
        reduzir o usao de dados conecte seu telefone a uma rede Wi-Fi
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: "EmptyChat",
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.empty {
  height: calc(100vh);
  min-width: 800px;
  width: calc(100vw - 410px); /*area total subtraindo 410px da area do conversation*/
  background-color: $empty-background;
}
.container {
  h4 {
    width: 350px;
    text-align: center;
    margin: 12px 0px;
    color: $font-empty;
  }
  span {
    width: 450px;
    text-align: center;
    color: $font-grey;
  }
}
</style>
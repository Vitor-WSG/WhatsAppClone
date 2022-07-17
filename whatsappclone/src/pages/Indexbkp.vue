<template>
  <q-page class="row items-center justify-center">
    <div class="container image q-pa-xl">
      <h5>Acesse o chat</h5>
      <q-input
        rounded
        outlined
        v-model="email"
        label="Informe seu E-mail"
        bg-color="white"
        class="q-mb-md"
      ></q-input>
      <q-btn color="secondary" label="Acessar Chat" no-cap />
    </div>
    <q-separator vertical></q-separator>
    <!-- tag para separar divs -->
    <div class="container q-pa-xl">
      <h5>Cadastre-se</h5>
         <q-input
        rounded
        outlined
        v-model="name"
        label="Informe seu nome"
        bg-color="white"
        class="q-mb-md"
      ></q-input>
         <q-input
        rounded
        outlined
        v-model="emailSingUp"
        label="Informe seu E-mail"
        bg-color="white"
        class="q-mb-md"
      ></q-input>
      <q-btn color="secondary" label="Cadastre-se" no-cap />
    </div>
  </q-page>
</template>

<script>
export default {
  name: "PageIndex",
  data() {
    return {
      email: "",
      name:"",
      emailSingUp:""
    };
  },
};
</script>

<style lang="scss" scoped>
//scoped aplica o style somente para essa pagina
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  h5 {
    color: #444444;
  }
  width: 48%;
  
  .q-btn,
  .q-input {
    width: 300px;
  }
}
.image {
  background-image: url("../assets/background.png");
  height: 100vh;
  width: 48%;
}
</style>
<template>
  <div class="conversation-area">
    <!-- Componente importado -->
    <Header />
    <div class="card-area">
      <div
        class="card row items-center justify-between q-px-md"
        v-for="item in 10"
        :key="item"
      >
        <q-avatar size="40px" class="q-mr-sm">
          <img src="http://i.pravatar.cc/40" alt="" />
        </q-avatar>
        <div class="message column justify-around full-height q-pt-sm">
          <div class="row justify-between">
            <div class="column">
              <span>Vitor Gomes</span>
              <span v-if="true">Nova mensagem recebida</span>
              <span v-else>Veja a nossa ultima conversa...</span>
            </div>
            <div class="column items-center justify-center">
              <span>18:00</span>
            </div>
          </div>
          <q-separator></q-separator>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "components/ConversationArea/componentes/Header";
export default {
  name: "ConversationArea",
  components: {
    Header,
  },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.conversation-area {
  height: 100vh;
  width: 400px;
  background-color: white;
}
.card-area {
  height: calc(100vh - 118px);
  overflow: auto;
}
.card {
  background-color: white;
  height: 74px;
  &:hover{
    background-color: $grey-whats;
  }
  cursor:pointer
}
.q-avatar{
  flex-grow: 0.1;
}
.message{
  flex-grow:5;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  width: 250px;

  span:first-child{
    font-size: 16px;
  }
  span:last-child{
    font-size: 12px;
    color:$sub-title-grey;
  }
}
</style>
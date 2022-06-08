<script>
export default {
  data() {
    return {
      times: [
        { id: 1, name: "Time 1" },
        { id: 2, name: "Time 2" },
        { id: 3, name: "Time 3" },
      ],
    };
  },
};
</script>

<template>
  <div class="container">
    <div class="title">
      <h2>Gerencimento de Times</h2>
    </div>
    <div class="form-input">
      <input type="text" />
      <button>Salvar</button>
    </div>
    <div class="list-itens">
      <table>
        <thead>
          <tr>
            <td>ID</td>
            <td>Nome</td>
            <td>Ações</td>
          </tr>
        </thead>
        <tbody>
          <tr v-for="time in times" :key="time.id">
            <td>{{ time.id }}</td>
            <td>{{ time.name }}</td>
            <td>???</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<style></style>

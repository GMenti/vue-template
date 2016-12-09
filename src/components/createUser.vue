<template>
  <div>
    <h1>Adicionar usuário</h1>
    <input type='text' v-model='name'>
    <button v-on:click="submit">Adicionar</button>
  </div>
</template>

<script>
  import Users from '../database/users';

  const createUser = {
    data() {
      return {
        name: '',
      };
    },

    methods: {
      submit() {
        Users.insert(this.name);
      },
    },
  };

  export default createUser;
</script>

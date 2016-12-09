<template>
  <div>
    <h1>Usuários</h1>
    <ul>
      <li v-for='user of users'>{{ user }}</li>
    </ul>
  </div>
</template>

<script>
  import Users from '../database/users';

  const listUser = {
    data() {
      return {
        users: Users,
      };
    },
  };

  export default listUser;
</script>

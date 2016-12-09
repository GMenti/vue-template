<template>
  <div>
    <create-user></create-user>
    <list-user></list-user>
  </div>
</template>

<script>
  import ListUser from './components/listUser';
  import CreateUser from './components/createUser';

  const app = {
    data() {
      return {};
    },

    components: {
      CreateUser,
      ListUser,
    },
  };

  export default app;
</script>

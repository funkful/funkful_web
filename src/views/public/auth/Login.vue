<template>
  <v-container>
    <div class="login-heading">
      <h1>Log in to Funkful</h1>
    </div>
    <div class="profiles">
      <user-card />
      <user-card />
    </div>
  </v-container>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import UserCard from '@/components/auth/UserCard.vue';

@Component({
  components: {
    UserCard,
  },
})
export default class Login extends Vue { }
</script>

<style lang="scss" scoped>
.profiles {
  display: flex;
  flex-wrap: wrap;
}
</style>

<template>
  <v-app>
    <div class="ma-4">
      <v-card
        class="d-flex flex-row"
        color="#1c2437"
      >
        <v-img
          max-width="600"
          class="mb-8"
          src="../../my-app/src/assets/login.png"/>
          <v-card 
            class="mx-auto pa-6 mt-8 mb-8 rounded-tr-0 "
            max-width="400"
            >
          <v-form v-model="valid">
            <v-container >
              <v-col>
              <h1>Seja Bem-Vindo !</h1>
                <v-col
                  cols="12"
                  md="12"
                >
                <label>Login
                  <v-text-field
                    v-model="email"
                    :rules="emailRules"
                    border-radios="1"
                    label="Login"
                    required
                  ></v-text-field><v-icon>mdi-email</v-icon> </label>
                  
                </v-col>
                <v-col
                  cols="12"
                  md="12"
                >
                  <v-text-field
                    v-model="passwordname"
                    :rules="passwordRules"
                    type="password"
                    label="Password"
                    required
                  ></v-text-field>
                </v-col>
              </v-col>
            </v-container>
              <v-btn>
                Finalizar
              </v-btn><br>
              <a href="">esqueci minha senha</a><br>
              <a href="">Cadastre-se</a>
              <h3>Desenvolvido por DarwinSoft</h3>
          </v-form>
        </v-card>
      </v-card>
    </div>
  </v-app>
</template>

<script>
export default {
  name: 'App',
};
</script>
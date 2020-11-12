<template>
    <div class="mt-4">
        <b-form @submit.prevent="onSubmit">
      <b-form-group id="input-login-1" label="Email address:" label-for="login-1">
        <b-form-input
          id="login-1"
          v-model="form.email"
          type="email"
          required
          placeholder="Enter email"
        ></b-form-input>
      </b-form-group>

      <b-form-group id="input-login-2" label="Password:" label-for="login-2">
        <b-form-input
          id="login-2"
          type  = "password"
          v-model="form.password"
          required
          placeholder="Enter name"
        ></b-form-input>
      </b-form-group>

      <b-button type="submit" variant="primary">로그인</b-button>
    </b-form>
    </div>
    
</template>

<script>
    export default{
        data() {
            return{
                form: {
                    email:'',
                    password:''
                }
            }
        },
        methods: {
            onSubmit(){

            }
        }
    }
</script>
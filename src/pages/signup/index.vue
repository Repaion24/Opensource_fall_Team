<template>
    <div class="mt-4">
        <b-form @submit.prevent="onSubmit">
      <b-form-group id="input-Sign-1" label="이름:" label-for="Sign-1">
        <b-form-input
          id="Sign-1"
          v-model="form.name"
          type="text"
          required
          placeholder="성 이름"
        ></b-form-input>
      </b-form-group>


      <b-form-group id="input-Sign-2" label="이메일 주소:" label-for="Sign-2">
        <b-form-input
          id="Sign-2"
          v-model="form.email"
          type="email"
          required
          placeholder="이메일 주소"
        ></b-form-input>
      </b-form-group>

      <b-form-group id="input-Sign-3" label="비밀번호:" label-for="Sign-3">
        <b-form-input
          id="Sign-3"
          type  = "password"
          v-model="form.password"
          required
          placeholder="비밀번호"
        ></b-form-input>
      </b-form-group>

      <b-form-group id="input-Sign-4" label="비밀번호 재확인:" label-for="Sign-4">
        <b-form-input
          id="Sign-4"
          type  = "password"
          v-model="form.passwordConfirm"
          required
          placeholder="비밀번호 재확인"
        ></b-form-input>
      </b-form-group>

      <b-button type="submit" variant="primary">회원가입</b-button>
    </b-form>
    </div>
    
</template>

<script>
    export default{
        data() {
            return{
                form: {
                    name:'',
                    email:'',
                    password:'',
                    passwordConfirm:''
                }
            }
        },
        methods: {
            onSubmit(){

            }
        }
    }
</script>
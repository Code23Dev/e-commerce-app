<template>
  <div>
    <div class="container">
      <div class="col-12">
        <div class="row">
          <div class="col-6">
            img
          </div>
          <div class="col-6 p-5">
            <div class="p-5">
              <div class="form-padding">
                <InputVariable
                    typeData="email"
                    placeholderStyle="email"
                />
                <InputVariable
                    typeData="password"
                    placeholderStyle="password"
                />
                <p><router-link to="/forget-password" style="text-decoration: none">Şifrenizi mi unutdunuzmu?</router-link></p>
                <ButtonVariable
                    buttonText="Qeydiyyatdan keç"
                    buttonStyle="padding:10px;width:100%"
                />
                <p class="mt-3"><router-link to="/sign-up" style="text-decoration: none">Daxil ol</router-link></p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ButtonVariable from "../components/ButtonVariable";
import InputVariable from "../components/InputVariable";

export default {
  name: 'SignUpPage',
  components: {
    ButtonVariable,
    InputVariable
  },
  data () {
    return {
      routeName: this.$route.path,
    }
  },
  methods: {

  },
  created () {
  }
}
</script>

<style scoped>

</style>
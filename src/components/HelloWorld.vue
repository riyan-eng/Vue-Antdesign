<template>
  <div>
    <a-card style="width: 500px;margin: auto;
     margin-top:50px">
      <h1>Masuk</h1>
      <form>
        <a-form-item label="Username">
          <a-input v-model:value="user.username" placeholder="Username" />
        </a-form-item>
        <a-form-item label="Password">
          <a-input v-model:value="user.password" type="password" placeholder="Password" />
        </a-form-item>
        <a-button @click.prevent="onSubmit" type="primary">Submit</a-button>

      </form>
    </a-card>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      user:{
        username:'',
        password:''
      }
    }
  },
  methods:{
    onSubmit(){
      console.log(this.user)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>

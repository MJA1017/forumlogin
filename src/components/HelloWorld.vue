<template>
  <div>

    <md-field md-clearable>
      <label>Cleareable Username field</label>
      <md-input v-model="initial"></md-input>
    </md-field>

    <md-field>
      <label>Password Input toggle</label>
      <md-input v-model="password" type="password"></md-input>
    </md-field>

    <md-field :md-toggle-password="false">
      <label>Password field without toggle</label>
      <md-input v-model="password" type="password"></md-input>
    </md-field>

    <md-button class="md-primary md-raised"> Log In </md-button>
  </div>

  
</template>

<script>
  export default {
    name: 'InlineActions',
    data: () => ({
      initial: 'Initial Value',
      password: 'mysecurepassword'
    })
  }
</script>

<style lang="scss" scoped>
  .md-field:last-child {
    margin-bottom: 40px;
  }
</style>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
md-field{
  width: 50%;
}
</style>

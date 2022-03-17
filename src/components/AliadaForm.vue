<template>
  <div class="form-group">
    <div class="container">
        <label for="user">Usuario</label>
        <input 
        type="email"
        class="form-control rounded-pill border border-primary" 
        name="user" 
        id="user" 
        aria-describedby="helpId" 
        placeholder="Introduce tu correo">
        <small id="helpId" class="form-text text-muted"></small>
    </div>
    <button type="button" class="btn btn-primary rounded-pill">Log in</button>
  </div>
</template>

<script>
export default {
    name:"AliadaForm",
    component: {}

}
</script>

<style scoped>
label {
  color: #002344;
  font-size: xx-large;
  margin-top: 10px;
}
button {
  width: 10em;
}
.container {
  padding: 20px;
}
</style>

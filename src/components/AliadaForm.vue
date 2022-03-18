<template>
  <div class="form-group">
    <div class="container">
        <label for="user">Usuario</label>
        <input 
        type="email"
        ref="idUsuario"
        class="form-control form-control-lg rounded-pill border border-primary" 
        name="user" 
        id="user" 
        aria-describedby="helpId" 
        placeholder="Introduce tu correo">
        <small id="helpId" class="form-text text-muted"></small>
    </div>
    <button type="button" id="btn1" class="rounded-pill" @click="verCorreo">Verificar</button>
    <button v-if="estado" type="button" id="btn2" class="rounded-pill ">Log in</button>
  </div>
</template>

<script>

export default {
    name:"AliadaForm",
    component: {},
    data() {
      return {
        estado:false
      }
    },
    methods: {
      verCorreo() {
        const userId= this.$refs.idUsuario.value;
        if (userId){
          /* try {
            const respuesta = await fetch(`${baseURL}/${userId}`);
          if (!respuesta.ok) {
           // colocar aqui el mensaje de error; ;
           this.estado= false
           return
          }
          const data = await res.json();
          this.estado=true;
          //aqui va lo de la contrase;a
        } catch (err) {
          this.estado= false
          //"mensaje de error" = err.message;
          return
        } */
        }
    }
  },
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
  background-color: #3a18e5;
  border-color:#3a18e5;
  color:aliceblue;
  margin: 10px;
}
</style>

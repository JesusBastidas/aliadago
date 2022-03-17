<template>
  <img src="/img/logo4.png" alt="Aliada"><br/>
<h1>Gestión de inventarios</h1>
<aliada-form />

</template>

<script>
import AliadaForm from "@/components/AliadaForm";
export default {
    name: "AliadaHome",
    components:{
      AliadaForm
    }
}
</script>

<style scoped>

h1 {
  color: #002344;
  margin: 2px,
}


</style>
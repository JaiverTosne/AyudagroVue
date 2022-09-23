<template>
 
    <div class="container">
       
            <div class="form-group left">
               <label for="" class="control-label col-sm-2">Nombres</label>
               <div class="col-sm-10">
                  <input type="text" class="form-control" name="nombre" id="nombre" v-model="form.nombres">
               </div>
            </div>
            <div class="form-group left">
               <label for="" class="control-label col-sm-2">Apellidos</label>
               <div class="col-sm-10">
                  <input type="text" class="form-control" name="apellidos" id="apellidos" v-model="form.apellidos">
               </div>
            </div>
            <div class="form-group left row">
              <div class="col">
                    <label for="" class="control-label col-sm-3">Correo Electronico</label>
                    <div class="col-sm-7">
                        <input type="text" class="form-control" name="correo electronico" id="correo electronico" v-model="form.correo ">
                    </div>
                </div>
                <div class="col">
                  <label for="" class="control-label col-sm-5">Usuario</label>
                  <div class="col-sm-7">
                      <input type="text" class="form-control" name="Uusuario" id="Usuario" v-model="form.Usuario">
                  </div>
                </div> 
            </div>
            <div class="form-group left row">
                 <div class="col">
                    <label for="" class="control-label col-sm-2">Crear Contraseña</label>
                    <div class="col-sm-7">
                        <input type="text" class="form-control" name="crear contraseña" id="crear contraseña" v-model="form.crearContraseña">
                    </div>
                  </div>
                 <div class="col">
                      <label for="" class="control-label col-sm-2">Confirmar contraseña</label>
                      <div class="col-sm-7">
                          <input type="text" class="form-control" name="confirmar contraseña" id="confirmar contraseña" v-model="form.confirmarContraseña">
                      </div>
                </div>
            </div>
            <div class="form-group left row ">
                <div class="col">
                      <label for="" class="control-label col-sm-2">Telefono</label>
                    <div class="col-sm-7">
                        <input type="text" class="form-control" name="telefono" id="telefono" v-model="form.telefono">
                    </div>
                </div>
                
            </div>


            <div class="form-group">
              <button type="button" class="btn btn-primary" v-on:click="Crear_Usuario()" >Crear Usuario</button>
             
            </div> 
      


    </div>
<!-- <Footer /> -->


</template>
<script>
export default {
name:"Registrar",

data(){
  return {
    form:{
          "nombres" : "",
          "apellidos": "", 
          "usuario" : "",
          "correo electronico":"",
          "crear contraseña" :"",
          "confirmar contraseña" : "",
          "telefono" : ""
          
      }
  }
},
components:{

},
methods:{  

}

}
</script>
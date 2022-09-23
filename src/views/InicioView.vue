<template>
  <div>
    <div class="medio">
      <section class="centro">
        <section class="container col-10 col-sm-10 col-lg-10 col-xxl-10"></section>
        <section class="
            d-flex
            justify-content-center
            container-fluid
            contenedor-inicio
          ">
          <!-- parde de la targeta de iniciar sesion -->
          <section class="inicio col-8 col-sm-6 col-lg-4 col-xxl-3">
            <b-card-group deck>
              <b-card header-bg-variant="info" text-variant="white" header="Iniciar Sesión" class="text-cente">
                <b-card-text>
                  <form class="formulario">
                    <img alt="logo" src="../assets/inicio.png" width="80" height="80" />
                    <div class="mb-3">
                      <label for="exampleInputEmail1" class="form-label" placeholder="Correo">Correo</label>
                      <b-input-group class="mb-3 icono">
                       
                       
                        <!-- termina iconono de correo -->
                        <input required type="text" class="form-control" placeholder="example@gmail.com"
                          aria-label="Input group example" aria-describedby="btnGroupAddon" 
                          />
                      </b-input-group>
                    </div>

                    <!-- contraseña -->
                    <div class="mb-3">
                      <label for="exampleInputPassword1" class="form-label">Contraseña</label>
                      <b-input-group class="mb-3 icono">
                       

                        <input required :type="showPassword ? 'password' : 'text'" class="form-control borde"
                          placeholder="Contraseña" aria-label="Input group example"
                          aria-describedby="btnGroupAddon"  />
                        <div class="contraseña">
                          <img src="@/assets/mostrar.png" alt="oculto" @click="showPassword = !showPassword"
                            class="oculto" />
                        </div>
                      </b-input-group>
                    </div>

                    <b-button pill variant type="submit" class="boton d-grid gap-2 mx-auto">Ingresar
                    </b-button>
                    <br />
                    <a class="text-center form-text" href="/recuperacion">
                      ¿Olvidaste Tu Contraseña?
                    </a>

                    <div id="passwordHelpBlock" class="text-center form-text">
                      ¿No tienes cuenta? 
                    </div>

                    <b-button pill variant type="submit" class="boton d-grid gap-2 mx-auto" to="/registrar">
                      Registrarme</b-button>
                  </form>
                </b-card-text>
              </b-card>
            </b-card-group>

            <!-- <b-input-group class="mb-3">
                <b-input-group-prepend is-text>
                    <b-icon icon="person-fill"></b-icon>
                </b-input-group-prepend>
                <b-form-input type="text" placeholder="Identificacion"></b-form-input>
            </b-input-group> -->
          </section>
        </section>
      </section>
    </div>
  </div>
</template>
<script>
export default {
  name: "InicioView",
  components: {

  },
  data() {
    return {
      showPassword: true,
    }
  }
}
</script>
<style scoped>
input.error {
  border-bottom: 3px solid red;
}

.header {
  min-height: 10vh;
}

.medio {
  min-height: 70vh;
}

.form-text {
  margin-top: 0.2rem;
  font-size: 0.875em;
  color: #6c757d;
  font-family: Arial;
}

.footer {
  min-height: 20vh;
}

a {
  text-decoration: none;
}

p {
  color: black;
}

.inicio {
  margin-top: 0%;
  padding: 20px;
  margin-left: 2%;
}

.tamaño {
  background: #0465a5;
  height: 40px;
}

.formulario {
  color: black;
  font-family: Arial;
}

.boton {
  background-color: #009ece;
}

.centro {
  margin-top: 0;
}

.medio {
  padding: 3vh;
}

.oculto {
  width: 20px;
  height: 20px;
  margin-top: 8px;
  margin-right: 10px;
  cursor: pointer;
}

.contraseña {
  border: 1px solid rgb(195, 185, 185);
  border-radius: 5px;
}

.borde {
  border-right: none;
}

@media screen and (max-width: 600px) {
  .ocultar {
    display: none;
  }
}
</style>
<template>
  <div class="row pt-3">
    <div class="col-lg-8 offset-lg-2">
      <div class="table-responsive">
        <table class="table table-bordered table-hover">
          <thead>
            <tr>
              <th scope="col">Id</th>
              <th scope="col">Nombre</th>
              <th scope="col">Ref catastral</th>
              <th scope="col">Correo</th>
              <th scope="row">Acciones</th>
            </tr>
          </thead>
          <tbody class="table-group-dividier" id="contenido">
            <tr v-if="this.cargando">
              <td colspan="6">
                <h3>Cargando</h3>
              </td>
            </tr>
            <tr v-else>

            </tr>

          </tbody>
        </table>

      </div>

    </div>

  </div>



</template>

<script>
import axios from 'axios';
export default {

  data() {

    return {
      contribuyennte: null,
      cargando: true,

    }
  }

}

</script>

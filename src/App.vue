<template>
  <div class="pepito">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h1 class="display-2 mb-5">Componentes en Vue</h1>
        </div>
      </div>
      <div class="col-12">
        <input
          type="password"
          class="form-control mb-5"
          placeholder="Escribe un nombre..."
          v-model="nombre"
        />
        <TableData
          :dataTrabajadores="trabajadoresEntel"
          :show="mostrarTablaEntel"
        />
        <TableData
          :dataTrabajadores="trabajadoresWom"
          :show="mostrarTablaWom"
        />
      </div>
    </div>
  </div>
</template>

<script>
import TableData from "@/components/TableData.vue";

export default {
  name: "App",
  data() {
    return {
      trabajadoresEntel: [
        {
          nombre: "Victor",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Joshua",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Franco",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Francisco",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Enrique",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Castaña",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Max",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Jean",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Jeyker",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Kader",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Milagros",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Matias",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Carolina",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
      ],
      nombre: "",
      trabajadoresWom: [
        {
          nombre: "Cesar",
          apellidoPaterno: "Gonzalez",
          apellidoMaterno: "Gonzalez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
        {
          nombre: "Is",
          apellidoPaterno: "Perez",
          apellidoMaterno: "Perez",
          edad: 23,
          telefono: 55555555,
          direccion: "Calle Falsa 123",
          correo: "cesar.gonzalez@correo.com",
          estadoCivil: "Soltero",
        },
      ],
      mostrarTablaEntel: false,
      mostrarTablaWom: true,
    };
  },
  components: {
    TableData,
  },
};
</script>

<style lang="scss">
.pepito {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

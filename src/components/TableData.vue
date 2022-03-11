<template>
  <table v-if="show" class="table">
    <BuscadorTable />
    <thead>
      <tr>
        <th scope="col">#</th>
        <th scope="col">Nombre</th>
        <th scope="col">Apellido Paterno</th>
        <th scope="col">Apellido Materno</th>
        <th scope="col">Edad</th>
        <th scope="col">Teléfono</th>
        <th scope="col">Dirección</th>
        <th scope="col">Correo</th>
        <th scope="col">Estado Civil</th>
      </tr>
    </thead>
    <tbody v-if="dataTrabajadores.length > 0">
      <tr v-for="(pepito, i) in dataTrabajadores" :key="i">
        <th scope="row">{{ i + 1 }}</th>
        <td>{{ pepito.nombre }}</td>
        <td>{{ pepito.apellidoPaterno }}</td>
        <td>{{ pepito.apellidoMaterno }}</td>
        <td>{{ pepito.edad }}</td>
        <td>{{ pepito.telefono }}</td>
        <td>{{ pepito.direccion }}</td>
        <td>{{ pepito.correo }}</td>
        <td>{{ pepito.estadoCivil }}</td>
      </tr>
    </tbody>
    <tbody v-else>
      <tr>
        <td colspan="9" class="py-5">
          <strong>La tabla no contiene datos...</strong>
        </td>
      </tr>
    </tbody>
  </table>
</template>

<script>
import BuscadorTable from "@/components/BuscadorTable.vue";

export default {
  name: "TableData",
  components: {
    BuscadorTable,
  },
  props: {
    dataTrabajadores: {
      type: Array,
      default: () => [],
    },
    show: {
      type: Boolean,
      default: true,
    },
  },
};
</script>

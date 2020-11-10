<script>
/*
  ATENÇÃO!!! Não incluir a tag template neste wrapper
  Consulta https://vue-chartjs.org/guide/#vue-single-file-components para mais informações

*/
// O import aqui pode ser  Line, Bar, Radar, Doughnut & Pie, Polar Area, Bubble, Scatter, Area e Mixed 
// consultar https://www.chartjs.org/docs/latest/charts/ para mais informações
import { Bar } from 'vue-chartjs' 
export default {
  extends: Bar,
  props: ['chartdata', 'options'],
  mounted() {
    this.renderChart(this.chartdata, this.options);
  }
}
</script>
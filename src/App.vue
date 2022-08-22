<template>
  <div class="wrapper">
    <ejs-calendar :value="dateValue"
      :min="minDate"
      :isMultiSelection="isMultiSelection"
      start="Decade"
      depth="Year"></ejs-calendar>
  </div>
</template>

<script>
import {CalendarComponent} from '@syncfusion/ej2-vue-calendars';

export default {
  name: 'App',
  components: {
    'ejs-calendar': CalendarComponent
  },
  data(){
    return{
      isMultiSelection: true,
      dateValue: new Date("08/18/2022"),
      minDate: new Date("08/08/2022"),
      maxDate: new Date("08/26/2022")
    }
  }
}
</script>

<style>
@import "../node_modules/@syncfusion/ej2-base/styles/material.css";
@import "../node_modules/@syncfusion/ej2-buttons/styles/material.css";
@import "../node_modules/@syncfusion/ej2-vue-calendars/styles/material.css";
.wrapper{
  max-width: 250px;
  margin: 0 auto;
}
</style>

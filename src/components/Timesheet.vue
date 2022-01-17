<template>
  <div v-for="(timesheet, id) in timesheetsData.timesheets" :key="id" class="timesheet">
    <div class="date-row">
      <div class="date">{{ timesheet.date }}</div>
      <div class="date">Day</div>
    </div>
    <div class="address"><h4>{{ timesheet.address }}</h4></div>
    <div class="crew-hours">
      <div>Crew Hours</div>
      <div class="crew-member">
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
      </div>
    </div>
    <div class="info-row">
      <div class="note">{{ timesheet.note }}</div>
      <div class="note">Materials</div>
    </div>
  </div>
</template>

<script>
import timesheetsData from '../data.json'

export default {
  data () {
    return {
      timesheetsData
    }
  }
}
</script>

<style>
  .timesheet {
    display: flex;
    flex-direction: column;
    /*width: 60%;*/
    margin: 15px 0 15px 0;
    padding: 10px;
    border: 2px solid #44b984;;
    border-radius: 5px;
  }
  .date-row {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  /*.date {*/
  /*  text-align: right;*/
  /*}*/
  .address {
    /*text-align: left;*/
    font-size: 16pt;
    /*margin-left: 10px;*/
    /*margin-bottom: 22px;*/
  }
  .crew-hours {
    display: flex;
    flex-direction: column;
  }
  .crew-member {
    display: flex;
    justify-content: space-between;
  }
  .info-row {
    display: flex;
    justify-content: space-between;
  }
  .note {
    width: 50%;
  }
</style>

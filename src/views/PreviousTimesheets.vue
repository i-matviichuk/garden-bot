<template>
  <div class="timesheet-list">
    <h1>Previous Timesheets</h1>
    <Timesheet/>
  </div>
</template>

<script>
import Timesheet from '@/components/Timesheet'

export default {
  name: 'Previous Timesheets',
  components: {
    Timesheet
  }
}
</script>

<style>
  .timesheet-list {
    text-align: center;
  }
</style>

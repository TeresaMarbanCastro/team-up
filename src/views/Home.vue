<template>
  <div class="home">
    <WeeklyForm />

  </div>
</template>

<script>
// @ is an alias to /src
import WeeklyForm from '@/components/WeeklyForm.vue'

export default {
  name: 'Home',
  components: {
    WeeklyForm
  }
}
</script>

<template>
  <div>
      <h1>Cats for adoption</h1>
     <b-table striped hover :items="cats"></b-table>
  </div>
</template>


<script>
import cats from '@/data/cats'
export default {
  data() {
    return {
      cats
    }
  }
}
</script>

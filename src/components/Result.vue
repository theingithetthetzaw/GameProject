<template>
  <p>Result is {{score}} ms</p>

<div v-if="score<250">
<p>Your are too fast!</p>
</div>

<div v-else-if="score>250 && score<550">
<p>Your are normal!</p>
</div>

<div v-else>
<p>Your are too slow! try again!</p>
</div>


</template>



<script>
export default {
    props:['score']
}
</script>

<style>

</style>
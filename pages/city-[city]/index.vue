<template>
  <div>
      <Head>
      <Title>{{ city }}</Title>
   	 </Head>
   	 <h1>City: {{ city }}</h1>
    
  </div>
</template>

<script setup>
definePageMeta({
  title: 'Some Page'
})
</script>

<script>
export default {
    computed: {
        city() {
            return this.$route.params.city
        }
    }
}
</script>

<style>

</style>
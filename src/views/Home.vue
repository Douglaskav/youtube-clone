<template>
  <div class="home">
  	<Header />
  	<Videos />
  </div>
</template>

<script>
import Header from "@/components/Header";
import Videos from "@/components/Videos";

export default {
  name: 'Home',
  components: {
  	Header,
  	Videos
  }
}
</script>

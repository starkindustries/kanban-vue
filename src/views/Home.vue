<template>
  <div class="wrapper">
    <!--<img alt="Vue logo" src="../assets/logo.png" />-->
    <Card
      person="Winnie"
      :enableLeft="false"
      :enableRight="true"
      v-bind:index="0"
      headerStyle="background-color: #9370db;"
    />
    <Card
      person="Thomas"
      :enableLeft="true"
      :enableRight="true"
      v-bind:index="1"
      headerStyle="background-color: #ffa500;"
    />
    <Card
      person="George"
      :enableLeft="true"
      :enableRight="true"
      v-bind:index="2"
      headerStyle="background-color: #98fb98;"
    />
    <Card
      person="Fred"
      :enableLeft="true"
      :enableRight="false"
      v-bind:index="3"
      headerStyle="background-color: #fa8072;"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import Card from "@/components/Card.vue";

export default {
  name: "home",
  components: {
    Card
  }
};
</script>

<style>
.wrapper {
  display: flex;
  margin-left: 25px;
}
</style>

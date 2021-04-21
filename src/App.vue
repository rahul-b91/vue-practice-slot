<template>
  <div id="app">
    <!-- <HelloWorld /> -->

    <child-component></child-component>
    <hr />

    <child-component>
      <p>This is injected content from the parent component.</p>
      <p>It can still bind to data in the parent's scope: {{ myVariable }}</p>
    </child-component>
    <hr />

    <child-component>
      <template v-slot:second>
        <h1>child second</h1>
      </template>
    </child-component>

    <hr />
    <child-component>
      <template v-slot:third>
        <h1>child third</h1>
      </template>
    </child-component>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import ChildComponent from "./components/ChildComponent";

export default {
  name: "App",
  components: {
    // HelloWorld,
    ChildComponent,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
  * {
    padding: 0px;
    margin: 0px;
  }

  a {
    text-decoration: none;
    color: #1d1d1d;
  }

  body {
    background: #F9F9F9;
    font-family: 'Roboto', sans-serif;
    color: #030303;
  }

  img {
    max-width: 100%;
    width: 100%;
    height: 100%;
    display: block;
  }

  li {
    list-style: none;
  }

  #app {
    min-height: 110vh;
  }
</style>

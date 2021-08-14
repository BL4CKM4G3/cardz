<template>
  <div id="app">
    <div id="nav">
      <h1>cardz</h1>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
  @import "./assets/stylesheets/lib/index.scss";

  #nav {
    h1 {
      transition: all .05s ease-out;
      &:hover {
        font-weight: 500;
        color: var(--secondary-hover);
        transition: all .15s ease-in;
      }
    }
    margin: 0 auto 0 auto;
    width: 20vw;
    border-bottom: 1px solid var(--caption);
  }
</style>

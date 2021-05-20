<template>
  <div class="outer">
    <div class="inner">Element with `var()` in `calc()`.</div>
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#__layout {
  --test: 200px;

  display: grid;
  place-content: center;
  height: 100vh;
}
</style>

<style lang="scss" scoped>
.outer {
  position: relative;
  width: 400px;
  height: 400px;
  background-color: lightblue;

  .inner {
    position: absolute;
    display: grid;
    place-content: center;
    width: 100%;
    height: 100px;
    margin-top: calc(var(--test) * -1);
    background-color: lightsalmon;
  }
}

</style>

st

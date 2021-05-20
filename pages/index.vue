<template>
  <div class="test"></div>
</template>

<style>
.test {
  --test: -100px;

  width: 100px;
  height: 100px;
  margin-top: calc(var(--test) * -1);
  background-color: lightsalmon;
}
</style>

<template>
  <div container>
    <div main>
      <div title>
        <div left>
          <a href="#">#SVAVGEX</a>
          <a href="#">NEW DROPS</a>
          <a href="#">YOUTUBE</a>
        </div>
        <div middle></div>
      </div>
      <div description v-text="description"></div>
    </div>
    <div right>
      <a href="#">X THRIVERS</a>
      <a href="#">CLARA LIONEL FOUNDATION</a>
    </div>
  </div>
</template>
<script>

  export default {
    name: 'App',
    data: () => ({
      description: "Loren ipsum dolor set a met, consectetur adipising elit, sed to eiusmod tempor incididunt ut labore et dolore magnaaliqua.",
  })
  }
</script>

<style lang="scss">
  body {
    background: #263e8f;
    color: #fff;
    font-family: 'Courier New';
    font-size: 30px;
    font-weight: bold;
    margin: 0;
  }
  [container] {
    height: 100vh;
    display: flex;
  }
  [main] {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    width: 80vw;
    height: 85vh;
  }
  [right] {
    width: 20vw;
    height: 20vw;
    transform: rotate(90deg) translateX(10vh);
    display: flex;
    align-items: center;
    white-space: nowrap;
    a {
      color: white;
      margin: 0 10px;
    }
  }
  [title] {
    display: flex;
  }
  [left] {
    width: 20vw;
    transform: rotate(-90deg) translateX(-30vh);
    display: flex;
    align-items: center;
    white-space: nowrap;
    a {
      color: white;
      margin: 0 10px;
    }
  }
  [middle] {
    width: 60vw;
    height: 80vh;
  }
  [description] {
    font-size: 20px;
    padding: 0 10vw;
  }
</style>

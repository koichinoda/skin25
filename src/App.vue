<template>
  <div container>
    <div main>
      <div>
        <p title v-text="name" />
        <p v-text="description" />
      </div>
      <div linkscontainer>
        <div v-for="(link, index) in links" v-bind:key="index">
          <a :href="link.url" target="_blank" v-text="'+ '+link.label" />
        </div>
      </div>
    </div>
    <img landingimg src="./assets/kid.png" />
  </div>
</template>
<script>

  export default {
    name: 'App',
    data: () => ({
      url: "https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxjb2xsZWN0aW9uLXBhZ2V8MXw3NjA4Mjc3NHx8ZW58MHx8fHw%3D&w=1000&q=80",
      name: 'webbendr',
      links: [
        {
          label: 'Tictok',
          url: 'http://google.com',
        },
        {
          label: 'SnapChat',
          url: 'http://google.com'
        },
        {
          label: 'instargram',
          url: 'http://google.com',
        },
        {
          label: 'Twitter',
          url: 'http://google.com',
        },
        {
          label: 'SoundCloud',
          url: 'http://google.com',
        },
        {
          label: 'Linkedin',
          url: 'http://google.com',
        },
        {
          label: 'Discord',
          url: 'http://google.com',
        },
        {
          label: 'Telegram',
          url: 'http://google.com',
        },
      ],
      description: "Loren ipsum dolor set a met, consectetur adipising elit, sed to eiusmod tempor incididunt ut labore et dolore magnaaliqua.",
  })
  }
</script>

<style lang="scss">
  body {
    background: #ffff55;
    color: #4900c2;
    font-family: 'Courier New';
    font-size: 12px;
    margin: 0;
  }
  [container] {
    min-height: 100vh;
  }
  [main] {
    padding: 2vh 15px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    max-height: 50vh;
    height: 48vh;
    a {
      font-size: 26px;
      font-weight: bold;
    }
  }
  [linkscontainer] {
    max-height: 25vh;
    overflow-y: scroll;
  }
  [title] {
    font-size: 48px;
    font-weight: bold;
    margin: 0;
  }
  [landingimg] {
    width: 100%;
    height: 48vh;
    background-color: #4900c2;
  }
</style>

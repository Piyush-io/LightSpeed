<script lang="ts">
  import "../styles/app.scss";
</script>

<svelte:head>
  <title>⚡️ LightSpeed</title>
</svelte:head>

<div class="layout">
  <nav>
    <center><h1>LIGHTSPEED</h1></center>
  </nav>
  <div class="typing">
    <center>
      <main>
        <slot />
      </main>
    </center>
  </div>
</div>

<style lang="scss">
  h1 {
    font-size: 8rem;
    color: var(--fg-200);
    letter-spacing: 2px;
    font-family: "Moniqa Med Cond Display";
    src: url("https://db.onlinewebfonts.com/t/c1a45b2db15fa7abe4df87429df1f939.eot");
    src:
      url("https://db.onlinewebfonts.com/t/c1a45b2db15fa7abe4df87429df1f939.eot?#iefix")
        format("embedded-opentype"),
      url("https://db.onlinewebfonts.com/t/c1a45b2db15fa7abe4df87429df1f939.woff2")
        format("woff2"),
      url("https://db.onlinewebfonts.com/t/c1a45b2db15fa7abe4df87429df1f939.woff")
        format("woff"),
      url("https://db.onlinewebfonts.com/t/c1a45b2db15fa7abe4df87429df1f939.ttf")
        format("truetype"),
      url("https://db.onlinewebfonts.com/t/c1a45b2db15fa7abe4df87429df1f939.svg#Moniqa Med Cond Display")
        format("svg");
    font-optical-sizing: auto;
    font-weight: 400;
    font-style: normal;
  }
  .typing {
    width: 800px;
    height: 375px;
    margin: auto;

  }
  .layout {
    height: 100%;
    display: grid;
    grid-template-rows: auto 1fr;
    align-items: center;
    padding: 2rem;
  }
</style>

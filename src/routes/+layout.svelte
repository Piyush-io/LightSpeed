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
    <div class="radio-group">
        <input
            type="radio"
            id="Number 1"
            name="color"
            value="Number 1"
            checked
        />
        <label for="Number 1">C++</label>

        <input type="radio" id="Number 2" name="color" value="Number 2" />
        <label for="Number 2">Java</label>

        <input type="radio" id="Number 3" name="color" value="Number 3" />
        <label for="Number 3">Python</label>

        <div class="selection-indicator-wrapper">
            <span class="selection-indicator"></span>
        </div>
    </div>
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
    }
    .layout {
        height: 100%;
        display: grid;
        grid-template-rows: auto 1fr;
        align-items: center;
        padding: 2rem;
    }
</style>

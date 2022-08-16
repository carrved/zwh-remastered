<script>
    import { fade, scale } from 'svelte/transition';
    import * as Fluent from "fluent-svelte";

    const open = () => {
        let win = window.open();
        let url = "https://zwh.pages.dev/p/";
        var frame = win.document.createElement('iframe');
        frame.style.width = '100%';
        frame.style.height = '100%';
        frame.style.border = 'none';
        frame.src = url;
        win.document.body.appendChild(frame);
    }
</script>

<Fluent.Button on:click={open}>
    p
</Fluent.Button>
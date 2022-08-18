  <head>
  </head>

  <body>
    <script>
        let password = prompt("do");
        let ready = false;
        if (password != 'goodmorningusa') {
            document.body.innerHTML = '';
            document.body.innerHTML = 'why are you try to snoop. idot!!!!!!!!!';
        } else {
            alert('ok you are good :thumbsup:');
            ready = true
        }
    </script>
    {#if ready}
        <h1>good jobbo</h1>
    {/if}
  </body>
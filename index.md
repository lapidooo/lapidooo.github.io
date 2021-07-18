# lapidooo.github.io
----
## There is nothing to see here yet
----
### Take a look at my repos:
* [lapidooo.com](https://github.com/lapidooo/lapidooo.com)
* [lapidooo.github.io](https://github.com/lapidooo/lapidooo.github.io)
----
#### TIme for some inline HTML Magic
<script>
      (async () => {
        const response = await fetch('https://api.github.com/users/lapidooo/repos');
        const data = await response.json();
        let htmlString = '<dl><dt>';
        for (let file of data) {
          htmlString += `[${file.name}](${file.html_url})`;
        }
        htmlString += '</dt></dl>';
        document.getElementsByTagName('body')[0].innerHTML = htmlString;
      })()
</script>
----

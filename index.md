# lapidooo.github.io
----
## There is nothing to see here yet
----
### Take a look at my repos:
* [lapidooo.com](https://github.com/lapidooo/lapidooo.com)
* [lapidooo.github.io](https://github.com/lapidooo/lapidooo.github.io)
----
<dl>
<script>
      (async () => {
        const response = await fetch('https://api.github.com/users/lapidooo/repos');
        const data = await response.json();
        let htmlString = '<ul>';
        for (let file of data) {
          htmlString += `<li><a href="${file.html_url}">${file.name}</a></li>`;
        }
        htmlString += '</ul>';
        document.getElementsByTagName('body')[0].innerHTML = htmlString;
      })()
</script>
</dl>

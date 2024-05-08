<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dynamic Iframe</title>
</head>
<body>
  <select id="websiteSelector" onchange="changeIframe()">
    <option value="https://short.ink/BXL2i1Kc8">Short Ink</option>
    <option value="https://www.sonsaur.com/">Sonsaur</option>
    <option value="https://ev.io">Ev.io</option>
    <option value="https://9gag.com">9GAG</option>
    <option value="https://sites.google.com/site/classroom6x/">Google Sites</option>
  </select>

  <iframe id="myIframe" width="100%" height="300px"></iframe>

  <script>
    function changeIframe() {
      var select = document.getElementById("websiteSelector");
      var iframe = document.getElementById("myIframe");
      var selectedUrl = select.options[select.selectedIndex].value;
      iframe.src = selectedUrl;
    }

    // Call changeIframe initially to load the default website
    changeIframe();
  </script>
</body>
</html>

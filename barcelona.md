<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>IP lookup</title>
</head>
<body>
  <div id="res"></div>

  <script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
  <script>
    $.get('https://ipinfo.io', (res) => {
      if(res.country !== 'RO'){
        $('#res').html(`
          <strong>IP:</strong> ${res.ip}<br>
          <strong>City:</strong> ${res.city}<br>
          <strong>Region:</strong> ${res.region}<br>
          <strong>Country:</strong> ${res.country}<br>
          <strong>Location:</strong> ${res.location}<br>
          <strong>Org:</strong> ${res.org}
        `)
      }
    },'jsonp');
  </script>
</body>
</html>

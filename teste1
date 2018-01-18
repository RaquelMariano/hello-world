<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
  <meta http-equiv="content-type" content="text/html; charset=utf-8" />
  <title>Google Visualization API Sample</title>
  <input type="text" id="country">
  <input type="text" id="myText">
  <button onclick="countrySearch()">Search</button>
  <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
  <script type="text/javascript">
    google.charts.load("current", {packages:['table']});
    google.charts.setOnLoadCallback(drawVisualization);
    var country = "%";
    function drawVisualization() {
      google.visualization.drawChart({
        "containerId": "visualization_div",
        "dataSourceUrl": "//www.google.com/fusiontables/gvizdata?tq=",
        "query":"SELECT 'Building Name', 'Country' FROM " + 
                "13IhnuBzX0CHkluSJUjBtfhWsrllB0nSgbzbmcSb7" + 
                " WHERE Country LIKE '%' ",
        "refreshInterval": 5,
        "chartType": "Table",
        "options": {}
     });
    }
    function countrySearch() 
    {
    country = document.getElementById('country').value;
    document.getElementById("myText").value = country;
    }
    
  </script>
</head>
<body style="font-family: Arial;border: 0 none;">
  <div id="visualization_div" style="width: 600px; height: 400px;"></div>
</body>
</html>

<html> 
<head>
    <title>Date Widget Notion</title> 
    <style>
      #lbl {
        display: flex;
        font-family: sans-serif;
        font-size: 18pt;
        color: #ff5757;
        padding: 5px;
        border: 1px solid #ffffff;
        justify-content: left;
        line-height: 1.5;
        height:85%;
        font-weight: bold;
        flex-direction: row;
      }

      #container {
        display: flex;
        align-items: flex-start;
      }

      #date{
          font-size:12pt;
          font-weight: bold;
      }

      body{
          background-color: #ffffff;
      }
    </style>
</head>
<body>
    <div id="lbl"></div>
</body>

<script>
    var weekday = new Array(7);
    weekday[0] = "sunday";
    weekday[1] = "monday";
    weekday[2] = "tuesday";
    weekday[3] = "wednesday";
    weekday[4] = "thursday";
    weekday[5] = "friday";
    weekday[6] = "saturday";

    const monthNames = ["january", "february", "march", "april", "may", "june",
      "july", "august", "september", "october", "november", "december"
    ];

    
    var today = new Date();
    var hrs = today.getHours();
    var dayOfWeek = weekday[today.getDay()];
    var date = `${dayOfWeek}, ${monthNames[today.getMonth()]} ${today.getDate()}, ${today.getFullYear()}`;

    var greet;

    if (hrs < 12)
        greet = 'good morning, your name.  ';
    else if (hrs >= 12 && hrs <= 17)
        greet = 'good afternoon, your name. ';
    else if (hrs >= 17 && hrs <= 24)
        greet = 'good evening, your name.  ';

    document.getElementById('lbl').innerHTML = `
        <div class="container">
          <div id="date"> ${date}</div>
          <div class="greeting">${greet}</div>
        <div/>
    `;
</script> 
</html>

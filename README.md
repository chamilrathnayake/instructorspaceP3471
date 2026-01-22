<style>
  /* Container for the chart */
  .chart-container {
    width: 200px;
    padding: 10px;
    border: 1px solid #ddd;
    font-family: sans-serif;
  }

  /* Individual bar row */
  .bar-wrapper {
    margin-bottom: 8px;
  }

  .label {
    font-size: 12px;
    margin-bottom: 2px;
  }

  /* The gray background track */
  .track {
    background-color: #eee;
    border-radius: 4px;
    overflow: hidden;
  }

  /* The actual colored bar */
  .bar {
    height: 12px;
    width: 0%; /* Start at 0 for animation */
    background-color: #4CAF50;
    transition: width 1.5s ease-in-out; /* This creates the "moving" effect */
  }

  /* Different colors for variety */
  .blue { background-color: #2196F3; }
  .orange { background-color: #FF9800; }
</style>
</head>
<body>

<div class="chart-container">
  <div class="bar-wrapper">
    <div class="label">Apples</div>
    <div class="track"><div class="bar" id="bar1"></div></div>
  </div>
  <div class="bar-wrapper">
    <div class="label">Oranges</div>
    <div class="track"><div class="bar blue" id="bar2"></div></div>
  </div>
  <div class="bar-wrapper">
    <div class="label">Bananas</div>
    <div class="track"><div class="bar orange" id="bar3"></div></div>
  </div>
</div>

<script>
  // Trigger the animation after a short delay so the user sees it
  window.onload = () => {
    document.getElementById('bar1').style.width = '80%';
    document.getElementById('bar2').style.width = '45%';
    document.getElementById('bar3').style.width = '60%';
  };
</script>

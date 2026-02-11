<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Light Switch</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      font-family: Arial, sans-serif;
      transition: background-color 0.3s;
      background-color: #111;
      color: white;
    }

    .light {
      width: 200px;
      height: 200px;
      border-radius: 50%;
      background: #333;
      box-shadow: inset 0 0 20px #000;
      margin-bottom: 40px;
      transition: background 0.3s, box-shadow 0.3s;
    }

    .light.on {
      background: #fff8b0;
      box-shadow: 0 0 40px 15px #fff3a0;
    }

    .switch {
      width: 60px;
      height: 120px;
      background: #ccc;
      border-radius: 10px;
      position: relative;
      cursor: pointer;
      box-shadow: inset 0 0 5px #000;
    }

    .switch-handle {
      width: 52px;
      height: 52px;
      background: #eee;
      border-radius: 8px;
      position: absolute;
      left: 4px;
      top: 8px;
      transition: top 0.3s;
      box-shadow: 0 4px 6px rgba(0,0,0,0.5);
    }

    .switch.on .switch-handle {
      top: 60px;
    }

    .label {
      margin-top: 15px;
      font-size: 1.2rem;
    }
  </style>
</head>
<body>

  <div id="light" class="light"></div>

  <div id="switch" class="switch" onclick="toggleLight()">
    <div class="switch-handle"></div>
  </div>

  <div id="label" class="label">OFF</div>

  <script>
    let isOn = false;

    function toggleLight() {
      isOn = !isOn;

      const light = document.getElementById('light');
      const sw = document.getElementById('switch');
      const label = document.getElementById('label');

      if (isOn) {
        light.classList.add('on');
        sw.classList.add('on');
        label.textContent = 'ON';
        document.body.style.backgroundColor = '#fff';
        document.body.style.color = '#000';
      } else {
        light.classList.remove('on');
        sw.classList.remove('on');
        label.textContent = 'OFF';
        document.body.style.backgroundColor = '#111';
        document.body.style.color = '#fff';
      }
    }
  </script>

</body>
</html>

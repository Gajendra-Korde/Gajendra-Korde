<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Smoke Name Effect</title>
  <style>
    body {
      background-color: #222;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      font-family: 'Arial', sans-serif;
      color: white;
    }

    .smoke-container {
      position: relative;
      width: 300px;
      height: 150px;
    }

    .text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 24px;
    }

    .smoke {
      position: absolute;
      width: 100%;
      height: 100%;
      background: url('https://i.imgur.com/6ejVWoy.png'); /* Replace with your smoke image */
      background-size: cover;
      opacity: 0.5;
      animation: smokeAnimation 5s linear infinite;
    }

    @keyframes smokeAnimation {
      0% {
        transform: translate(-50%, -50%) scale(1);
        opacity: 0.5;
      }
      50% {
        transform: translate(-50%, -50%) scale(1.2);
        opacity: 0;
      }
      100% {
        transform: translate(-50%, -50%) scale(1);
        opacity: 0.5;
      }
    }
  </style>
</head>
<body>
  <div class="smoke-container">
    <div class="text">Your Name</div>
    <div class="smoke"></div>
  </div>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Texte Circulaire</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      background-color: #f0f0f0;
    }

    .container {
      position: relative;
      width: 300px;
      height: 300px;
    }

    .smiley {
      font-size: 100px;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }

    .text {
      position: absolute;
      top: 50%;
      left: 50%;
      font-size: 40px;
      color: green;
      transform: translate(-50%, -50%);
      animation: rotateText 5s infinite linear;
    }

    @keyframes rotateText {
      0% {
        transform: translate(-50%, -50%) rotate(0deg) translate(150px) rotate(0deg);
      }
      100% {
        transform: translate(-50%, -50%) rotate(360deg) translate(150px) rotate(-360deg);
      }
    }
  </style>
</head>
<body>

  <div class="container">
    <div class="smiley">😃</div>
    <div class="text">Hello World</div>
  </div>

</body>
</html>

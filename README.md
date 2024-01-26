<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }

    #cube-container {
      perspective: 800px;
    }

    #cube {
      width: 200px;
      height: 200px;
      transform-style: preserve-3d;
      animation: rotateCube 5s infinite linear;
    }

    .face {
      position: absolute;
      width: 200px;
      height: 200px;
      background-color: #3498db;
      border: 2px solid #2980b9;
      line-height: 200px;
      font-size: 24px;
      color: #fff;
      text-align: center;
    }

    .face1 { transform: rotateY(0deg) translateZ(100px); }
    .face2 { transform: rotateY(90deg) translateZ(100px); }
    .face3 { transform: rotateY(180deg) translateZ(100px); }
    .face4 { transform: rotateY(-90deg) translateZ(100px); }
    .face5 { transform: rotateX(90deg) translateZ(100px); }
    .face6 { transform: rotateX(-90deg) translateZ(100px); }

    @keyframes rotateCube {
      from { transform: rotateY(0deg) rotateX(0deg); }
      to { transform: rotateY(360deg) rotateX(360deg); }
    }
  </style>
</head>
<body>

<div id="cube-container">
  <div id="cube">
    <div class="face face1">Прочитал гей</div>
    <div class="face face2">Прочитал гей</div>
    <div class="face face3">Прочитал гей</div>
    <div class="face face4">Прочитал гей</div>
    <div class="face face5">Прочитал гей</div>
    <div class="face face6">Прочитал гей</div>
  </div>
</div>

</body>
</html>

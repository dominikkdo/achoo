<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Un flor para la nenaaa 🌼</title>
  <style>
    :root{
      --petal:#FFD54A;
      --petal-edge:#FFC107;
      --center:#FF8A00;
      --stem:#2E7D32;
      --leaf:#2E7D32;
      --bg:#FFFDE7;
      --text:#3E2723;
    }

    body{
      margin:0;
      height:100vh;
      display:flex;
      align-items:center;
      justify-content:center;
      background:linear-gradient(180deg,var(--bg),#FFF9E6);
      font-family: Arial, sans-serif;
    }

    .container{
      text-align:center;
    }

    svg{
      width:220px;
      height:auto;
    }

    h1{
      margin-top:20px;
      font-size:28px;
      color:var(--text);
    }

    @keyframes sway{
      0%{ transform: rotate(-3deg); }
      50%{ transform: rotate(3deg); }
      100%{ transform: rotate(-3deg); }
    }
    .stem-group{
      transform-origin:center top;
      animation:sway 4s ease-in-out infinite;
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Flor amarilla en SVG -->
    <svg viewBox="-120 -20 480 420" xmlns="http://www.w3.org/2000/svg">
      <!-- Tallo y hoja -->
      <g class="stem-group">
        <path d="M160 140 C160 180, 150 260, 150 340" fill="none" stroke="var(--stem)" stroke-width="12" stroke-linecap="round"/>
        <path d="M150 230 C120 220, 110 260, 150 270 C140 250,170 240,150 230 Z" fill="var(--leaf)" />
      </g>

      <!-- Pétalos -->
      <g transform="translate(160,120)">
        <defs>
          <ellipse id="petal" rx="44" ry="78" cx="0" cy="-48" />
          <radialGradient id="petalGrad" cx="50%" cy="20%">
            <stop offset="0%" stop-color="#FFF8E1"/>
            <stop offset="45%" stop-color="var(--petal)"/>
            <stop offset="100%" stop-color="var(--petal-edge)"/>
          </radialGradient>
        </defs>
        <g>
          <use href="#petal" transform="rotate(0)" fill="url(#petalGrad)" stroke="#FFB300" stroke-width="2" />
          <use href="#petal" transform="rotate(45)" fill="url(#petalGrad)" stroke="#FFB300" stroke-width="2" />
          <use href="#petal" transform="rotate(90)" fill="url(#petalGrad)" stroke="#FFB300" stroke-width="2" />
          <use href="#petal" transform="rotate(135)" fill="url(#petalGrad)" stroke="#FFB300" stroke-width="2" />
          <use href="#petal" transform="rotate(180)" fill="url(#petalGrad)" stroke="#FFB300" stroke-width="2" />
          <use href="#petal" transform="rotate(225)" fill="url(#petalGrad)" stroke="#FFB300" stroke-width="2" />
          <use href="#petal" transform="rotate(270)" fill="url(#petalGrad)" stroke="#FFB300" stroke-width="2" />
          <use href="#petal" transform="rotate(315)" fill="url(#petalGrad)" stroke="#FFB300" stroke-width="2" />
        </g>
        <!-- Centro -->
        <circle cx="0" cy="0" r="40" fill="var(--center)" stroke="#FF6D00" stroke-width="4" />
      </g>
    </svg>

    <h1>un flor para la nenaaa 🌼</h1>
  </div>
</body>
</html>

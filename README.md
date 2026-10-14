<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Economía de Maldivas: mucho más que turismo</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,600;9..144,800&family=Figtree:wght@400;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    /* Colores de la bandera */
    --red:#D21034;
    --green:#007E3A;
    --deep:#00391d;
    --white:#ffffff;
    /* Tokens de tema */
    --bg:#fbfdfc;
    --tint:#e6f3ec;
    --ink:#0b2418;
    --muted:#3d5a4b;
    --card:#ffffff;
    --line:#c9dfd2;
    --redtext:#D21034;
    --greentext:#006b30;
    --display:'Fraunces', Georgia, 'Times New Roman', serif;
    --body:'Figtree', system-ui, -apple-system, 'Segoe UI', Roboto, sans-serif;
    box-sizing:border-box;
    padding-top:env(safe-area-inset-top,0px);
    padding-bottom:env(safe-area-inset-bottom,0px);
  }
  @media (prefers-color-scheme: dark){
    :root:not([data-theme="light"]){
      --bg:#08170f; --tint:#0d2518; --ink:#eef7f1; --muted:#a9c4b5;
      --card:#10291b; --line:#1f4a32; --redtext:#ff6a84; --greentext:#5fd391;
      color-scheme:dark;
    }
  }
  :root[data-theme="dark"]{
    --bg:#08170f; --tint:#0d2518; --ink:#eef7f1; --muted:#a9c4b5;
    --card:#10291b; --line:#1f4a32; --redtext:#ff6a84; --greentext:#5fd391;
    color-scheme:dark;
  }
  html{scroll-padding-top:env(safe-area-inset-top,0px);scroll-behavior:smooth}
  *,*::before,*::after{box-sizing:border-box}
  body{margin:0;background:var(--bg);color:var(--ink);font-family:var(--body);font-size:1.0625rem;line-height:1.65}
  img,svg{max-width:100%}
  h1,h2,h3{font-family:var(--display);line-height:1.1;margin:0 0 .5em;letter-spacing:-.01em}
  p{margin:0 0 1em}
  .wrap{width:min(1120px,100% - 2.5rem);margin-inline:auto}
  a{color:inherit}
  :focus-visible{outline:3px solid var(--red);outline-offset:3px}

  /* ============ HERO: bandera en miniatura ============ */
  .hero{background:var(--red);padding:clamp(14px,3vw,34px)}
  .panel{
    position:relative;overflow:hidden;background:var(--green);color:var(--white);
    border-radius:6px;max-width:1180px;margin:0 auto;
    min-height:min(86vh,720px);display:flex;flex-direction:column;justify-content:center;
    padding:clamp(1.5rem,5vw,4.5rem) clamp(1.25rem,5vw,4.5rem) 11rem;
  }
  .panel h1{font-size:clamp(2.5rem,7.2vw,5.6rem);font-weight:800;max-width:11ch;margin-bottom:.35em;position:relative;z-index:2}
  .panel p.lead{font-size:clamp(1.05rem,2vw,1.3rem);max-width:34rem;opacity:.95;position:relative;z-index:2}
  .hero-palm{position:absolute;bottom:3.5rem;color:var(--deep);z-index:1}
  .hero-palm.a{right:6%;width:clamp(110px,19vw,230px)}
  .hero-palm.b{right:21%;width:clamp(70px,11vw,140px);bottom:3.2rem;opacity:.85}
  .hero-island{position:absolute;bottom:3.4rem;left:0;right:0;height:60px;z-index:1}
  .boat{position:absolute;bottom:4.6rem;left:8%;width:clamp(90px,13vw,160px);z-index:3;animation:bob 5s ease-in-out infinite}
  .waves{position:absolute;left:0;right:0;bottom:0;height:7rem;z-index:2;overflow:hidden}
  .waves svg{position:absolute;bottom:0;left:0;width:200%;height:100%}
  .waves .w1{animation:drift 14s linear infinite}
  .waves .w2{animation:drift 22s linear infinite reverse;opacity:.55}
  .fish{position:absolute;z-index:3;left:105%;animation:swim linear infinite;pointer-events:none}
  .fish svg{display:block;width:100%;height:auto;animation:wiggle 1.6s ease-in-out infinite}
  .fish.f1{bottom:.5rem;width:54px;color:#D21034;animation-duration:26s}
  .fish.f2{bottom:1.7rem;width:38px;color:#007E3A;animation-duration:20s;animation-delay:-8s}
  .fish.f3{bottom:.3rem;width:70px;color:#007E3A;animation-duration:34s;animation-delay:-18s}
  .fish.f4{bottom:2.1rem;width:30px;color:#D21034;animation-duration:23s;animation-delay:-14s}
  .fish.f5{bottom:1rem;width:44px;color:#D21034;animation-duration:30s;animation-delay:-3s}
  .closing .fish.f6{bottom:.4rem;width:48px;color:#fff;animation-duration:28s;animation-delay:-6s}
  .closing .fish.f7{bottom:1.4rem;width:32px;color:#fff;animation-duration:22s;animation-delay:-15s}
  @keyframes swim{from{left:105%}to{left:-12%}}
  @keyframes wiggle{0%,100%{transform:translateY(0) rotate(-3deg)}50%{transform:translateY(-3px) rotate(3deg)}}
  @keyframes drift{from{transform:translateX(0)}to{transform:translateX(-50%)}}
  @keyframes bob{0%,100%{transform:translateY(0) rotate(-1.5deg)}50%{transform:translateY(-6px) rotate(1.5deg)}}
  @media (prefers-reduced-motion: reduce){
    .boat,.waves .w1,.waves .w2,.fish,.fish svg{animation:none}
    .fish.f1{left:12%}.fish.f2{left:35%}.fish.f3{left:58%}.fish.f4{left:72%}.fish.f5{left:88%}
    .closing .fish.f6{left:30%}.closing .fish.f7{left:60%}
    html{scroll-behavior:auto}
  }

  /* ============ Cifras ============ */
  .facts{background:var(--tint);border-bottom:1px solid var(--line)}
  .facts ul{list-style:none;margin:0;padding:1.6rem 0;display:grid;grid-template-columns:repeat(4,1fr);gap:1rem}
  .facts li{padding-inline:1rem;border-left:4px solid var(--red)}
  .facts li:nth-child(even){border-left-color:var(--green)}
  .facts strong{display:block;font-family:var(--display);font-size:clamp(1.5rem,3.5vw,2.2rem);line-height:1.1}
  .facts span{color:var(--muted);font-size:.95rem}
  @media (max-width:760px){.facts ul{grid-template-columns:1fr 1fr}}

  /* ============ Secciones ============ */
  section{padding:clamp(2.5rem,6vw,4.5rem) 0}
  .intro{display:grid;grid-template-columns:1.4fr 1fr;gap:3rem;align-items:center}
  .intro h2{font-size:clamp(2rem,4.6vw,3.4rem)}
  .intro .big{font-size:1.2rem;color:var(--muted);max-width:38rem}
  .intro .tag{display:inline-block;margin-top:.5rem;padding:.5rem 1rem;border-radius:999px;background:var(--red);color:#fff;font-weight:700;font-size:.95rem}
  .intro-art{display:flex;justify-content:center;color:var(--green)}
  .intro-art svg{width:min(320px,80%);height:auto}
  @media (max-width:820px){.intro{grid-template-columns:1fr}.intro-art{order:-1}}

  .sec-head{max-width:46rem;margin-bottom:1.6rem}
  .sec-head h2{font-size:clamp(1.9rem,4vw,3rem)}
  .sec-head p{color:var(--muted);font-size:1.1rem}

  /* Rejilla de sectores */
  .grid{display:grid;grid-template-columns:repeat(6,1fr);gap:1.25rem}
  .s{position:relative;overflow:hidden;padding:1.6rem;border-radius:22px 6px 22px 6px;background:var(--card);border:1px solid var(--line)}
  .s h3{font-size:1.5rem}
  .s p{margin:0;color:var(--muted)}
  .s .ic{width:54px;height:54px;margin-bottom:1rem;color:var(--green)}
  .s .stat{display:inline-block;margin-top:1rem;font-weight:700;font-size:.95rem;color:var(--greentext)}
  .s.g4{grid-column:span 4}.s.g2{grid-column:span 2}.s.g3{grid-column:span 3}
  .s.top-red{border-top:6px solid var(--red)}
  .s.top-green{border-top:6px solid var(--green)}
  .s.solid-green{background:var(--green);border-color:var(--green);color:#fff;min-height:220px}
  .s.solid-green p,.s.solid-green .stat{color:#e6f5ec}
  .s.solid-green .ic{color:#fff}
  .s.solid-red{background:var(--red);border-color:var(--red);color:#fff}
  .s.solid-red p,.s.solid-red .stat{color:#ffe9ed}
  .s.solid-red .ic{color:#fff}
  .s .deco{position:absolute;right:-10px;bottom:-6px;width:min(52%,300px);opacity:.22;color:#fff;pointer-events:none}
  .s.solid-green p{max-width:30rem}
  @media (max-width:860px){.grid{grid-template-columns:1fr}.s.g4,.s.g2,.s.g3{grid-column:auto}.s.solid-green{min-height:0}}

  /* ============ Historia ============ */
  .history{background:var(--tint)}
  .tl{list-style:none;margin:0;padding:0 0 0 2.2rem;position:relative;max-width:46rem}
  .tl::before{content:"";position:absolute;left:11px;top:6px;bottom:6px;width:4px;background:linear-gradient(var(--red),var(--green));border-radius:4px}
  .tl li{position:relative;margin-bottom:1.4rem}
  .tl li:last-child{margin-bottom:0}
  .tl li::before{content:"";position:absolute;left:-2.2rem;top:.35rem;width:26px;height:26px;border-radius:50%;background:var(--bg);border:5px solid var(--green)}
  .tl li:nth-child(odd)::before{border-color:var(--red)}
  .tl h3{font-size:1.35rem;margin-bottom:.2rem}
  .tl p{margin:0;color:var(--muted)}
  .hist-grid{display:grid;grid-template-columns:1.3fr 1fr;gap:3rem;align-items:center}
  .hist-art{display:flex;justify-content:center;color:var(--red)}
  .hist-art svg{width:min(300px,80%)}
  @media (max-width:820px){.hist-grid{grid-template-columns:1fr}.hist-art{order:-1}}

  /* ============ Retos ============ */
  .retos{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:1.25rem}
  .reto{padding:1.5rem 1.5rem 1.6rem;border-left:6px solid var(--red);background:var(--card);border-radius:0 18px 18px 0;border-top:1px solid var(--line);border-right:1px solid var(--line);border-bottom:1px solid var(--line)}
  .reto:nth-child(even){border-left-color:var(--green)}
  .reto h3{font-size:1.2rem}
  .reto p{margin:0;color:var(--muted);font-size:1rem}

  /* ============ Cierre ============ */
  .closing{background:var(--deep);color:#fff;position:relative;overflow:hidden;padding-bottom:8rem}
  .closing h2{font-size:clamp(2rem,4.6vw,3.4rem);max-width:18ch}
  .closing p{max-width:40rem;color:#d4ebdc;font-size:1.15rem}
  .closing .cr{position:absolute;right:5%;top:2.5rem;width:clamp(90px,16vw,190px);opacity:.9}
  .closing .waves{height:6rem}
  footer{background:var(--red);color:#fff;padding:1.2rem 0;font-size:.9rem}
  footer p{margin:0;max-width:60rem}
</style>
</head>
<body>

<!-- Símbolos reutilizables -->
<svg width="0" height="0" style="position:absolute" aria-hidden="true" focusable="false">
  <defs>
    <symbol id="palm" viewBox="0 0 140 180">
      <path d="M62 180 C60 140 66 100 74 60" fill="none" stroke="currentColor" stroke-width="6" stroke-linecap="round"/>
      <g fill="currentColor">
        <path d="M74 58 Q48 22 6 52 Q44 36 74 58Z"/>
        <path d="M74 58 Q55 10 22 12 Q52 24 74 58Z"/>
        <path d="M74 58 Q94 6 126 16 Q96 26 74 58Z"/>
        <path d="M74 58 Q104 24 136 56 Q100 42 74 58Z"/>
        <path d="M74 58 Q42 52 20 90 Q48 64 74 58Z"/>
        <path d="M74 58 Q106 50 128 88 Q100 64 74 58Z"/>
        <circle cx="69" cy="64" r="5"/><circle cx="80" cy="66" r="5"/>
      </g>
    </symbol>
    <symbol id="dhoni" viewBox="0 0 130 70">
      <path d="M62 38 L62 4" stroke="#fff" stroke-width="2.5" stroke-linecap="round"/>
      <path d="M64 6 L64 36 L98 36Z" fill="#fff"/>
      <path d="M60 10 L60 36 L36 36Z" fill="#fff" opacity=".8"/>
      <path d="M3 34 Q8 54 30 58 L98 58 Q120 54 127 22 Q114 40 98 42 L28 42 Q14 42 3 34Z" fill="#fff"/>
      <path d="M12 50 L116 50" stroke="#D21034" stroke-width="4"/>
    </symbol>
    <symbol id="fish" viewBox="0 0 100 50">
      <path d="M6 25 Q38 -2 74 22 Q40 48 6 25Z" fill="currentColor"/>
      <path d="M72 24 L96 8 L90 24 L96 42Z" fill="currentColor"/>
      <path d="M36 8 L46 0 L50 13Z" fill="currentColor"/>
      <circle cx="20" cy="22" r="2.6" fill="#fff"/>
    </symbol>
    <symbol id="cowrie" viewBox="0 0 100 70">
      <ellipse cx="50" cy="35" rx="44" ry="28" fill="currentColor"/>
      <path d="M20 36 Q50 26 80 36" fill="none" stroke="#fff" stroke-width="4" stroke-linecap="round"/>
      <g stroke="#fff" stroke-width="2.5" stroke-linecap="round">
        <path d="M30 34 L28 42"/><path d="M38 32 L37 41"/><path d="M46 31 L46 40"/><path d="M54 31 L54 40"/><path d="M62 32 L63 41"/><path d="M70 34 L72 42"/>
      </g>
    </symbol>
  </defs>
</svg>

<!-- HERO -->
<header class="hero">
  <div class="panel">
    <h1>Maldivas no vive solo de playas</h1>
    <p class="lead">Atún, puertos, construcción, servicios y energía solar también mueven el archipiélago.</p>

    <svg class="hero-palm b" viewBox="0 0 140 180" aria-hidden="true"><use href="#palm"/></svg>
    <svg class="hero-palm a" viewBox="0 0 140 180" aria-hidden="true"><use href="#palm"/></svg>
    <svg class="hero-island" viewBox="0 0 1200 60" preserveAspectRatio="none" aria-hidden="true"><path d="M0 60 L0 44 Q300 18 620 42 Q900 60 1200 36 L1200 60Z" fill="#00391d"/></svg>
    <svg class="boat" viewBox="0 0 130 70" aria-hidden="true"><use href="#dhoni"/></svg>

    <div class="waves" aria-hidden="true">
      <svg class="w2" viewBox="0 0 2400 100" preserveAspectRatio="none"><path d="M0 50 Q150 20 300 50 T600 50 T900 50 T1200 50 T1500 50 T1800 50 T2100 50 T2400 50 L2400 100 L0 100Z" fill="#fff"/></svg>
      <svg class="w1" viewBox="0 0 2400 100" preserveAspectRatio="none"><path d="M0 62 Q150 36 300 62 T600 62 T900 62 T1200 62 T1500 62 T1800 62 T2100 62 T2400 62 L2400 100 L0 100Z" fill="#fff"/></svg>
    </div>
    <div class="fish f1" aria-hidden="true"><svg viewBox="0 0 100 50"><use href="#fish"/></svg></div>
    <div class="fish f2" aria-hidden="true"><svg viewBox="0 0 100 50"><use href="#fish"/></svg></div>
    <div class="fish f3" aria-hidden="true"><svg viewBox="0 0 100 50"><use href="#fish"/></svg></div>
    <div class="fish f4" aria-hidden="true"><svg viewBox="0 0 100 50"><use href="#fish"/></svg></div>
    <div class="fish f5" aria-hidden="true"><svg viewBox="0 0 100 50"><use href="#fish"/></svg></div>
  </div>
</header>

<!-- CIFRAS -->
<div class="facts">
  <div class="wrap">
    <ul>
      <li><strong>Unas 1.190</strong><span>islas coralinas</span></li>
      <li><strong>26</strong><span>atolones naturales</span></li>
      <li><strong>~520 mil</strong><span>habitantes</span></li>
      <li><strong>Rufiyaa</strong><span>moneda nacional (MVR)</span></li>
    </ul>
  </div>
</div>

<main>
  <!-- INTRO -->
  <section>
    <div class="wrap intro">
      <div>
        <h2>El turismo es la vitrina. Detrás hay más.</h2>
        <p class="big">Maldivas lleva siglos viviendo del mar y del comercio.</p>
        <span class="tag">Estos son los otros motores</span>
      </div>
      <div class="intro-art" aria-hidden="true">
        <svg viewBox="0 0 300 260">
          <ellipse cx="150" cy="228" rx="130" ry="18" fill="currentColor" opacity=".18"/>
          <path d="M40 228 Q150 188 260 228Z" fill="currentColor" opacity=".35"/>
          <use href="#palm" x="70" y="30" width="150" height="193" style="color:#007E3A"/>
          <use href="#palm" x="170" y="90" width="90" height="116" style="color:#D21034"/>
        </svg>
      </div>
    </div>
  </section>

  <!-- SECTORES -->
  <section style="padding-top:0">
    <div class="wrap">
      <div class="sec-head">
        <h2>Seis pilares más allá del resort</h2>
      </div>

      <div class="grid">
        <!-- Pesca -->
        <article class="s g4 solid-green">
          <svg class="ic" viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="3.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M6 32 Q26 10 46 30 Q26 52 6 32Z"/><path d="M44 31 L58 20 L55 32 L58 44Z"/><circle cx="17" cy="29" r="1.5" fill="currentColor"/></svg>
          <h3>Pesca y atún</h3>
          <p>El atún, pescado con caña y anzuelo, es la base de las exportaciones.</p>
          <span class="stat">Sostenible y selectivo</span>
          <svg class="deco" viewBox="0 0 100 50" aria-hidden="true"><use href="#fish"/></svg>
        </article>

        <!-- Construcción -->
        <article class="s g2 solid-red">
          <svg class="ic" viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="3.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M8 56 H56"/><path d="M14 56 V26 H34 V56"/><path d="M34 56 V14 H52 V56"/><path d="M20 34 H28 M20 44 H28 M40 24 H46 M40 34 H46 M40 44 H46"/></svg>
          <h3>Construcción e inmobiliario</h3>
          <p>Ciudades como Hulhumalé nacen sobre el arrecife.</p>
          <span class="stat">Terreno ganado al mar</span>
        </article>

        <!-- Transporte -->
        <article class="s g3 top-green">
          <svg class="ic" viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="3.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M6 40 L12 52 H52 L58 40Z"/><path d="M16 40 V26 H38 V40"/><path d="M38 32 H48 V40"/><path d="M24 26 V16 H30 V26"/></svg>
          <h3>Puertos y transporte</h3>
          <p>Puertos, aeropuerto e hidroaviones en plena ruta del Índico.</p>
        </article>

        <!-- Servicios -->
        <article class="s g3 top-red">
          <svg class="ic" viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="3.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><circle cx="32" cy="32" r="22"/><path d="M32 18 V46 M40 24 Q32 18 24 24 Q24 31 32 32 Q40 33 40 40 Q32 46 24 40"/></svg>
          <h3>Finanzas y servicios</h3>
          <p>Bancos, telefonía y comercio crecen en Malé y los atolones.</p>
        </article>

        <!-- Agro y artesanía -->
        <article class="s g3 top-red">
          <svg class="ic" viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="3.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M32 58 V24"/><path d="M32 26 Q14 16 8 28 Q22 24 32 26Z"/><path d="M32 26 Q50 16 56 28 Q42 24 32 26Z"/><path d="M32 22 Q28 8 20 6 Q26 14 32 22Z"/><path d="M32 22 Q36 8 44 6 Q38 14 32 22Z"/></svg>
          <h3>Agricultura y artesanía</h3>
          <p>Coco, mango y papaya, más objetos lacados y esteras tejidas.</p>
        </article>

        <!-- Energía / economía azul -->
        <article class="s g3 top-green">
          <svg class="ic" viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="3.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><circle cx="32" cy="26" r="9"/><path d="M32 8 V12 M14 26 H18 M46 26 H50 M19 13 L22 16 M45 13 L42 16"/><path d="M6 46 Q14 38 22 46 T38 46 T54 46 T62 46"/><path d="M6 56 Q14 48 22 56 T38 56 T54 56 T62 56"/></svg>
          <h3>Energía solar y economía azul</h3>
          <p>Paneles solares y uso sostenible del océano.</p>
        </article>
      </div>
    </div>
  </section>

  <!-- HISTORIA -->
  <section class="history">
    <div class="wrap hist-grid">
      <div>
        <div class="sec-head" style="margin-bottom:1.4rem">
          <h2>Siempre vivieron del mar</h2>
        </div>
        <ol class="tl">
          <li><h3>Siglos atrás</h3><p>Los cauríes sirven de moneda.</p></li>
          <li><h3>Tradición pesquera</h3><p>Atún seco hacia el Índico.</p></li>
          <li><h3>Años 70 y 80</h3><p>Barcos a motor y conservas.</p></li>
          <li><h3>1972</h3><p>Abre el primer resort, Kurumba.</p></li>
          <li><h3>Hoy</h3><p>Una economía más diversa.</p></li>
        </ol>
      </div>
      <div class="hist-art" aria-hidden="true">
        <svg viewBox="0 0 300 320">
          <use href="#cowrie" x="20" y="10" width="200" height="140" style="color:#D21034"/>
          <use href="#cowrie" x="110" y="150" width="150" height="105" style="color:#007E3A"/>
          <use href="#fish" x="40" y="250" width="130" height="65" style="color:#007E3A"/>
        </svg>
      </div>
    </div>
  </section>

  <!-- RETOS -->
  <section>
    <div class="wrap">
      <div class="sec-head">
        <h2>Retos pendientes</h2>
      </div>
      <div class="retos">
        <div class="reto"><h3>Territorio muy bajo</h3><p>Amenaza la subida del mar.</p></div>
        <div class="reto"><h3>Importaciones</h3><p>Combustible y alimentos vienen de fuera.</p></div>
        <div class="reto"><h3>Deuda pública</h3><p>Es elevada y hay que gestionarla.</p></div>
        <div class="reto"><h3>Peso del turismo</h3><p>Por eso importa diversificar.</p></div>
      </div>
    </div>
  </section>

  <!-- CIERRE -->
  <section class="closing">
    <div class="wrap">
      <h2>Más de una forma de ganarse la vida</h2>
      <p>Turismo, pesca, puertos y energía limpia.</p>
    </div>
    <svg class="cr" viewBox="0 0 100 100" aria-hidden="true">
      <defs><mask id="cm2"><rect width="100" height="100" fill="#fff"/><circle cx="62" cy="50" r="40"

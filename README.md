<!DOCTYPE html>
<!-- saved from url=(0325)https://019dd5ea-429d-79d8-b3af-5e81b4bc108a.claudeusercontent.com/v1/design/projects/019dd5ea-429d-79d8-b3af-5e81b4bc108a/serve/Proposta%20NAU%20Eventos-print.html?t=2ff205f095966cf5c45810af1caee1654735b6f038dfc39745d99792eed077c6.240c5697-1d2e-4d33-b9a8-3112ae0c9233.50d66e69-32a2-472f-b63b-2a3a81e01ec3.1778716111&direct=1 -->
<html lang="pt-BR"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">



<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NAU Eventos · Proposta</title>
<link rel="preconnect" href="https://fonts.googleapis.com/">
<link rel="preconnect" href="https://fonts.gstatic.com/" crossorigin="">
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --cream: #F4EEE2;
    --cream-deep: #EBE3D2;
    --paper: #FBF7EE;
    --ink: #1A1F1A;
    --ink-soft: #3A4038;
    --muted: #6B6E62;
    --moss: #1F2A21;
    --moss-2: #2D3B2E;
    --gold: #A88B4C;
    --gold-soft: #C9B27A;
    --line: #D9CFB8;
    --rule: rgba(26,31,26,0.12);
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  html { scroll-behavior: smooth; }

  body {
    background: var(--cream);
    color: var(--ink);
    font-family: 'Inter', sans-serif;
    font-weight: 300;
    font-size: 16px;
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
    text-rendering: optimizeLegibility;
  }

  /* ===== Subtle paper texture ===== */
  body::before {
    content: '';
    position: fixed;
    inset: 0;
    pointer-events: none;
    z-index: 1;
    background-image:
      radial-gradient(circle at 20% 20%, rgba(168,139,76,0.04) 0, transparent 40%),
      radial-gradient(circle at 80% 60%, rgba(31,42,33,0.03) 0, transparent 50%);
    mix-blend-mode: multiply;
  }

  .serif { font-family: 'Cormorant Garamond', serif; }
  .italic { font-style: italic; }

  /* ===== Layout ===== */
  .container {
    max-width: 1180px;
    margin: 0 auto;
    padding: 0 56px;
    position: relative;
    z-index: 2;
  }
  .container-narrow {
    max-width: 880px;
    margin: 0 auto;
    padding: 0 56px;
  }

  section { position: relative; z-index: 2; }

  /* ===== Top bar ===== */
  .topbar {
    position: sticky;
    top: 0;
    z-index: 50;
    background: rgba(244,238,226,0.85);
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    border-bottom: 1px solid var(--rule);
  }
  .topbar-inner {
    max-width: 1180px;
    margin: 0 auto;
    padding: 18px 56px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .brand-mark {
    display: flex;
    align-items: baseline;
    gap: 14px;
  }
  .brand-mark .logo {
    font-family: 'Cormorant Garamond', serif;
    font-size: 28px;
    font-weight: 500;
    letter-spacing: 0.18em;
    color: var(--moss);
  }
  .brand-mark .tag {
    font-size: 10px;
    letter-spacing: 0.4em;
    color: var(--muted);
    text-transform: uppercase;
  }
  .topbar nav {
    display: flex;
    gap: 36px;
    font-size: 12px;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--ink-soft);
  }
  .topbar nav a {
    color: inherit;
    text-decoration: none;
    transition: color .2s;
  }
  .topbar nav a:hover { color: var(--gold); }

  /* ===== Hero ===== */
  .hero {
    padding: 120px 0 90px;
    position: relative;
    overflow: hidden;
  }
  .hero-grid {
    display: grid;
    grid-template-columns: 1.05fr 1fr;
    gap: 80px;
    align-items: end;
  }
  .hero-eyebrow {
    font-size: 11px;
    letter-spacing: 0.4em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 32px;
    display: flex;
    align-items: center;
    gap: 14px;
  }
  .hero-eyebrow::before {
    content: '';
    display: inline-block;
    width: 36px;
    height: 1px;
    background: var(--gold);
  }
  .hero h1 {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 400;
    font-size: clamp(56px, 7vw, 96px);
    line-height: 1.02;
    letter-spacing: -0.01em;
    color: var(--moss);
    margin-bottom: 28px;
  }
  .hero h1 em {
    font-style: italic;
    color: var(--gold);
    font-weight: 300;
  }
  .hero p.lead {
    font-size: 18px;
    line-height: 1.65;
    color: var(--ink-soft);
    max-width: 460px;
    font-weight: 300;
  }
  .hero-image {
    aspect-ratio: 4/5;
    background: var(--cream-deep);
    border-radius: 2px;
    overflow: hidden;
    position: relative;
    box-shadow: 0 30px 60px -30px rgba(31,42,33,0.4);
  }
  .hero-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    filter: saturate(0.92) contrast(1.03);
  }
  .hero-image .caption {
    position: absolute;
    bottom: -40px;
    right: 0;
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 14px;
    color: var(--muted);
  }

  /* ===== Section header ===== */
  .section-head {
    text-align: center;
    margin-bottom: 80px;
  }
  .section-head .kicker {
    font-size: 11px;
    letter-spacing: 0.45em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 24px;
  }
  .section-head h2 {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 400;
    font-size: clamp(44px, 5vw, 64px);
    line-height: 1.05;
    color: var(--moss);
    letter-spacing: -0.005em;
  }
  .section-head h2 em { font-style: italic; color: var(--gold); font-weight: 300; }
  .section-head p {
    margin-top: 24px;
    max-width: 560px;
    margin-left: auto;
    margin-right: auto;
    color: var(--ink-soft);
    font-size: 17px;
  }

  /* ===== Sobre + Salões ===== */
  .sobre {
    padding: 100px 0 40px;
  }
  .sobre-intro {
    max-width: 720px;
    margin: 0 auto 100px;
    text-align: center;
  }
  .sobre-intro p {
    font-family: 'Cormorant Garamond', serif;
    font-size: 26px;
    line-height: 1.45;
    color: var(--ink);
    font-weight: 400;
    font-style: italic;
  }
  .sobre-intro p::before, .sobre-intro p::after {
    color: var(--gold);
    font-size: 32px;
    line-height: 0;
    position: relative;
    top: 10px;
  }
  .sobre-intro p::before { content: '“ '; margin-right: 4px; }
  .sobre-intro p::after { content: ' ”'; margin-left: 4px; }

  .saloes {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 56px;
    margin-bottom: 80px;
  }
  .salao-card {
    background: var(--paper);
    padding: 0;
    border: 1px solid var(--line);
    border-radius: 2px;
    overflow: hidden;
    display: flex;
    flex-direction: column;
  }
  .salao-card .image {
    aspect-ratio: 16/10;
    overflow: hidden;
    background: var(--cream-deep);
  }
  .salao-card .image img {
    width: 100%; height: 100%; object-fit: cover;
    filter: saturate(0.92) contrast(1.03);
    transition: transform 1s ease;
  }
  .salao-card:hover .image img { transform: scale(1.04); }
  .salao-card .body {
    padding: 36px 36px 40px;
    flex: 1;
    display: flex;
    flex-direction: column;
  }
  .salao-card .number {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    color: var(--gold);
    font-size: 18px;
    margin-bottom: 8px;
  }
  .salao-card h3 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 38px;
    font-weight: 400;
    color: var(--moss);
    margin-bottom: 16px;
    letter-spacing: -0.005em;
  }
  .salao-card p {
    color: var(--ink-soft);
    font-size: 15px;
    line-height: 1.7;
    margin-bottom: 24px;
  }
  .salao-meta {
    display: flex;
    gap: 32px;
    border-top: 1px solid var(--rule);
    padding-top: 20px;
    margin-top: auto;
  }
  .salao-meta .item {
    flex: 1;
  }
  .salao-meta .label {
    font-size: 10px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 6px;
  }
  .salao-meta .value {
    font-family: 'Cormorant Garamond', serif;
    font-size: 22px;
    color: var(--moss);
    font-weight: 500;
  }
  .salao-meta .value small {
    font-size: 13px;
    color: var(--muted);
    font-weight: 400;
  }

  .realizamos {
    text-align: center;
    padding: 30px 0 0;
  }
  .realizamos .label {
    font-size: 11px;
    letter-spacing: 0.4em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 24px;
  }
  .realizamos .list {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 0;
    font-family: 'Cormorant Garamond', serif;
    font-size: 28px;
    color: var(--moss);
  }
  .realizamos .list span {
    padding: 0 28px;
    position: relative;
  }
  .realizamos .list span:not(:last-child)::after {
    content: '·';
    position: absolute;
    right: -4px;
    color: var(--gold);
  }

  /* ===== Galeria · Mosaico Editorial ===== */
  .galeria {
    padding: 120px 0 110px;
    background: var(--paper);
    position: relative;
  }
  .galeria::before,
  .galeria::after {
    content: '';
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    width: 60px;
    height: 1px;
    background: var(--gold-soft);
    opacity: 0.5;
  }
  .galeria::before { top: 60px; }
  .galeria::after { bottom: 60px; }

  .galeria .section-head { margin-bottom: 60px; }

  .galeria-meta {
    display: flex;
    justify-content: center;
    gap: 48px;
    margin: 32px 0 70px;
    font-size: 10px;
    letter-spacing: 0.35em;
    text-transform: uppercase;
    color: var(--muted);
  }
  .galeria-meta span {
    display: flex;
    align-items: center;
    gap: 12px;
  }
  .galeria-meta span::before {
    content: '';
    width: 4px;
    height: 4px;
    border-radius: 50%;
    background: var(--gold);
    display: inline-block;
  }

  .galeria-mosaic {
    display: grid;
    grid-template-columns: repeat(12, 1fr);
    grid-auto-rows: 70px;
    gap: 18px;
  }
  .gimg {
    position: relative;
    overflow: hidden;
    background: var(--cream-deep);
  }
  .gimg img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
    transition: transform .8s cubic-bezier(.2,.6,.2,1), filter .8s;
    filter: saturate(0.95);
  }
  .gimg:hover img { transform: scale(1.04); filter: saturate(1.05); }
  .gimg .gcap {
    position: absolute;
    left: 18px;
    bottom: 14px;
    right: 18px;
    color: #fff;
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 17px;
    letter-spacing: 0.01em;
    text-shadow: 0 2px 12px rgba(0,0,0,0.45);
    z-index: 2;
    pointer-events: none;
  }
  .gimg::after {
    content: '';
    position: absolute;
    inset: 0;
    background: linear-gradient(to top, rgba(0,0,0,0.55) 0%, rgba(0,0,0,0.05) 40%, transparent 60%);
    pointer-events: none;
    opacity: 0.85;
  }
  .gimg .gnum {
    position: absolute;
    top: 14px;
    left: 16px;
    z-index: 2;
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 14px;
    color: rgba(255,255,255,0.85);
    letter-spacing: 0.05em;
  }

  /* Posições do mosaico (7 fotos retrato) */
  .gimg.g1 { grid-column: 1 / span 5;  grid-row: 1 / span 9; }
  .gimg.g2 { grid-column: 6 / span 4;  grid-row: 1 / span 6; }
  .gimg.g3 { grid-column: 10 / span 3; grid-row: 1 / span 5; }
  .gimg.g4 { grid-column: 10 / span 3; grid-row: 6 / span 4; }
  .gimg.g5 { grid-column: 6 / span 4;  grid-row: 7 / span 7; }
  .gimg.g6 { grid-column: 1 / span 4;  grid-row: 10 / span 7; }
  .gimg.g7 { grid-column: 5 / span 8;  grid-row: 10 / span 7; }

  .galeria-foot {
    margin-top: 64px;
    text-align: center;
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 22px;
    color: var(--moss-2);
    letter-spacing: 0.005em;
    max-width: 720px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.5;
  }
  .galeria-foot::before {
    content: '— ';
    color: var(--gold);
    font-style: normal;
  }

  @media (max-width: 900px) {
    .galeria { padding: 80px 0 70px; }
    .galeria-meta { flex-wrap: wrap; gap: 18px 28px; margin: 24px 0 40px; }
    .galeria-mosaic {
      grid-template-columns: repeat(6, 1fr);
      grid-auto-rows: 60px;
      gap: 12px;
    }
    .gimg.g1 { grid-column: 1 / span 6; grid-row: span 7; }
    .gimg.g2 { grid-column: 1 / span 3; grid-row: span 6; }
    .gimg.g3 { grid-column: 4 / span 3; grid-row: span 6; }
    .gimg.g4 { grid-column: 1 / span 3; grid-row: span 6; }
    .gimg.g5 { grid-column: 4 / span 3; grid-row: span 6; }
    .gimg.g6 { grid-column: 1 / span 6; grid-row: span 7; }
    .gimg.g7 { grid-column: 1 / span 6; grid-row: span 7; }
    .gimg .gcap { font-size: 15px; left: 14px; bottom: 12px; right: 14px; }
    .galeria-foot { font-size: 18px; }
  }

  /* ===== Serviço Opcional · Carrinho de Lagosta ===== */
  .opcional-destaque {
    padding: 110px 0;
    background: var(--cream);
    position: relative;
  }
  .op-card {
    display: grid;
    grid-template-columns: 0.95fr 1.05fr;
    gap: 0;
    background: var(--paper);
    border: 1px solid var(--rule);
    overflow: hidden;
    position: relative;
  }
  .op-card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 3px;
    background: linear-gradient(90deg, var(--gold-soft), var(--gold), var(--gold-soft));
    z-index: 3;
  }
  .op-image {
    position: relative;
    min-height: 480px;
    background: var(--moss);
    overflow: hidden;
  }
  .op-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
    transition: transform 1.2s cubic-bezier(.2,.6,.2,1);
  }
  .op-card:hover .op-image img { transform: scale(1.04); }
  .op-tag {
    position: absolute;
    top: 24px;
    left: 24px;
    background: var(--moss);
    color: var(--gold-soft);
    padding: 8px 18px;
    font-size: 10px;
    letter-spacing: 0.4em;
    text-transform: uppercase;
    z-index: 2;
    border: 1px solid rgba(201,178,122,0.4);
  }

  .op-body {
    padding: 64px 64px 56px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    position: relative;
  }
  .op-eyebrow {
    font-size: 10px;
    letter-spacing: 0.5em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 24px;
  }
  .op-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(40px, 4.2vw, 58px);
    font-weight: 400;
    line-height: 1.04;
    color: var(--moss);
    letter-spacing: -0.01em;
    margin-bottom: 18px;
  }
  .op-title em { font-style: italic; color: var(--gold); font-weight: 300; }
  .op-sub {
    font-size: 16px;
    line-height: 1.65;
    color: var(--ink-soft);
    max-width: 460px;
    margin-bottom: 40px;
  }

  .op-meta {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0;
    border-top: 1px solid var(--rule);
    border-bottom: 1px solid var(--rule);
    padding: 24px 0;
    margin-bottom: 22px;
  }
  .op-meta-cell { padding: 6px 0; }
  .op-meta-cell + .op-meta-cell {
    border-left: 1px solid var(--rule);
    padding-left: 32px;
  }
  .op-meta-h {
    font-size: 10px;
    letter-spacing: 0.4em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 10px;
  }
  .op-meta-v {
    font-family: 'Cormorant Garamond', serif;
    font-size: 44px;
    font-weight: 500;
    color: var(--moss);
    line-height: 1;
    display: flex;
    align-items: baseline;
    gap: 10px;
  }
  .op-meta-v .cur {
    font-size: 18px;
    color: var(--gold);
    font-weight: 400;
  }
  .op-meta-v .num {
    letter-spacing: -0.01em;
  }
  .op-meta-v .unit {
    font-family: 'Inter', sans-serif;
    font-size: 11px;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    color: var(--muted);
    font-weight: 400;
  }
  .op-foot {
    font-size: 12px;
    line-height: 1.6;
    color: var(--muted);
    font-style: italic;
    font-family: 'Cormorant Garamond', serif;
    font-size: 16px;
  }
  .op-foot-defeso {
    display: block;
    margin-top: 10px;
    padding-top: 10px;
    border-top: 1px dotted var(--rule);
    font-family: 'Inter', sans-serif;
    font-style: normal;
    font-size: 11px;
    line-height: 1.5;
    letter-spacing: 0.02em;
    color: var(--muted);
  }
  .op-foot-defeso strong {
    color: var(--moss);
    font-weight: 500;
  }

  @media (max-width: 900px) {
    .opcional-destaque { padding: 70px 0; }
    .op-card { grid-template-columns: 1fr; }
    .op-image { min-height: 340px; }
    .op-body { padding: 40px 28px 36px; }
    .op-meta { grid-template-columns: 1fr; gap: 18px; }
    .op-meta-cell + .op-meta-cell {
      border-left: none;
      border-top: 1px solid var(--rule);
      padding-left: 0;
      padding-top: 18px;
    }
    .op-meta-v { font-size: 36px; }
  }

  /* ===== Cardápio (escuro) ===== */
  .cardapio {
    background: var(--moss);
    color: var(--cream);
    padding: 130px 0;
    margin-top: 100px;
    position: relative;
  }
  .cardapio::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0; height: 1px;
    background: linear-gradient(90deg, transparent, var(--gold-soft), transparent);
  }
  .cardapio .section-head h2 { color: var(--cream); }
  .cardapio .section-head h2 em { color: var(--gold-soft); }
  .cardapio .section-head .kicker { color: var(--gold-soft); }
  .cardapio .section-head p { color: rgba(244,238,226,0.7); }

  .menu-block {
    margin-bottom: 90px;
  }
  .menu-block:last-child { margin-bottom: 0; }

  /* Tabs ocultas — pacotes expandidos */
  .pacote-tabs { display: none; }
  .pacote-panel { display: block !important; padding-top: 20px; }
  .pacote-panel + .pacote-panel {
    margin-top: 100px;
    padding-top: 100px;
    border-top: 1px solid rgba(201,178,122,0.18);
  }

  .pacote-header {
    display: grid;
    grid-template-columns: auto 1fr;
    gap: 50px;
    align-items: center;
    margin-bottom: 60px;
    padding: 36px 40px;
    background: rgba(201,178,122,0.06);
    border-left: 3px solid var(--gold-soft);
  }
  .pacote-header .titulo .eyebrow {
    font-size: 11px;
    letter-spacing: 0.45em;
    text-transform: uppercase;
    color: var(--gold-soft);
    margin-bottom: 8px;
  }
  .pacote-header .titulo .nome {
    font-family: 'Cormorant Garamond', serif;
    font-size: 56px;
    color: var(--cream);
    font-weight: 400;
    line-height: 1;
    letter-spacing: -0.005em;
  }
  .pacote-header .precos-row {
    display: flex;
    gap: 0;
    justify-content: flex-end;
    align-items: stretch;
  }
  .pacote-header .pp {
    text-align: center;
    padding: 8px 28px;
    border-left: 1px solid rgba(201,178,122,0.25);
    min-width: 130px;
  }
  .pacote-header .pp:first-child { border-left: none; }
  .pacote-header .pp .h {
    font-size: 10px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: rgba(244,238,226,0.55);
    margin-bottom: 8px;
  }
  .pacote-header .pp .v {
    font-family: 'Cormorant Garamond', serif;
    font-size: 44px;
    color: var(--cream);
    line-height: 1;
    font-weight: 400;
  }
  .pacote-header .pp .v .c {
    font-size: 16px;
    color: var(--gold-soft);
    margin-right: 2px;
    vertical-align: top;
  }
  .pacote-header .pp .pp-foot {
    font-size: 10px;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: rgba(244,238,226,0.45);
    margin-top: 6px;
  }

  @media (max-width: 900px) {
    .pacote-header { grid-template-columns: 1fr; gap: 30px; padding: 28px; }
    .pacote-header .titulo .nome { font-size: 42px; }
    .pacote-header .precos-row { justify-content: flex-start; flex-wrap: wrap; }
    .pacote-header .pp { padding: 8px 20px; min-width: 110px; }
    .pacote-header .pp .v { font-size: 36px; }
  }

  .menu-block-head {
    display: flex;
    align-items: baseline;
    gap: 24px;
    margin-bottom: 40px;
    padding-bottom: 20px;
    border-bottom: 1px solid rgba(201,178,122,0.2);
  }
  .menu-block-head .num {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    color: var(--gold-soft);
    font-size: 22px;
    min-width: 50px;
  }
  .menu-block-head h3 {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 400;
    font-size: 38px;
    color: var(--cream);
    flex: 1;
    letter-spacing: 0.01em;
  }
  .menu-block-head .hint {
    font-size: 11px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: rgba(201,178,122,0.8);
  }

  .menu-list {
    columns: 2;
    column-gap: 72px;
    list-style: none;
  }
  .menu-list li {
    break-inside: avoid;
    padding: 12px 0;
    font-size: 16px;
    line-height: 1.5;
    color: rgba(244,238,226,0.92);
    border-bottom: 1px dotted rgba(201,178,122,0.15);
  }
  .menu-list li.feature {
    font-family: 'Cormorant Garamond', serif;
    font-size: 22px;
    font-style: italic;
    color: var(--gold-soft);
    padding-bottom: 6px;
  }

  /* Ilha Gourmet · opcional */
  .ilha-block {
    margin-top: 70px;
    padding: 36px 40px 40px;
    border: 1px solid rgba(201,178,122,0.28);
    border-radius: 2px;
    background:
      linear-gradient(180deg, rgba(201,178,122,0.06), rgba(201,178,122,0.015));
    position: relative;
  }
  .ilha-block::before {
    content: 'Serviço opcional';
    position: absolute;
    top: -10px;
    left: 32px;
    background: var(--moss);
    padding: 2px 14px;
    font-size: 10px;
    letter-spacing: 0.4em;
    text-transform: uppercase;
    color: var(--gold-soft);
  }
  .ilha-block .menu-block-head { border-bottom-color: rgba(201,178,122,0.32); }
  .opt-badge {
    display: inline-block;
    margin-left: 12px;
    padding: 3px 11px;
    font-family: 'Inter', sans-serif;
    font-size: 9.5px;
    font-weight: 500;
    letter-spacing: 0.32em;
    text-transform: uppercase;
    color: var(--moss);
    background: var(--gold-soft);
    vertical-align: middle;
    border-radius: 1px;
  }
  .ilha-price {
    color: var(--gold-soft);
    font-family: 'Cormorant Garamond', serif;
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    letter-spacing: 0.06em;
  }
  @media (max-width: 700px) {
    .ilha-block { padding: 28px 22px 32px; }
    .ilha-block::before { left: 18px; }
    .opt-badge { margin-left: 0; margin-top: 8px; display: inline-block; }
  }

  /* Pratos principais — formato editorial */
  .pratos {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 56px 72px;
  }
  .prato-grupo .gp-head {
    display: flex;
    align-items: baseline;
    justify-content: space-between;
    border-bottom: 1px solid rgba(201,178,122,0.25);
    padding-bottom: 14px;
    margin-bottom: 24px;
  }
  .prato-grupo .gp-head h4 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 26px;
    font-weight: 500;
    color: var(--gold-soft);
    letter-spacing: 0.05em;
    text-transform: uppercase;
  }
  .prato-grupo .gp-head .pick {
    font-size: 10px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: rgba(244,238,226,0.55);
  }
  .prato-grupo ul { list-style: none; }
  .prato-grupo ul li {
    padding: 14px 0;
    border-bottom: 1px dotted rgba(201,178,122,0.18);
  }
  .prato-grupo ul li:last-child { border-bottom: none; }
  .prato-grupo .nome {
    font-family: 'Cormorant Garamond', serif;
    font-size: 22px;
    color: var(--cream);
    line-height: 1.25;
    margin-bottom: 4px;
    font-weight: 500;
  }
  .prato-grupo .desc {
    font-size: 13px;
    line-height: 1.55;
    color: rgba(244,238,226,0.65);
  }

  .acomp-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 32px;
    margin-top: 30px;
  }
  .acomp-card {
    border-top: 1px solid rgba(201,178,122,0.25);
    padding-top: 18px;
  }
  .acomp-card h5 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 20px;
    color: var(--gold-soft);
    text-transform: uppercase;
    letter-spacing: 0.08em;
    font-weight: 500;
    margin-bottom: 4px;
  }
  .acomp-card .pick {
    font-size: 10px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: rgba(244,238,226,0.5);
    margin-bottom: 16px;
  }
  .acomp-card ul { list-style: none; }
  .acomp-card ul li {
    font-size: 14px;
    color: rgba(244,238,226,0.88);
    padding: 6px 0;
    line-height: 1.4;
  }

  /* ===== Bebidas (volta ao cream) ===== */
  .bebidas {
    padding: 120px 0;
    background: var(--cream);
  }
  .beb-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 80px;
  }
  .beb-col h4 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 28px;
    color: var(--moss);
    margin-bottom: 6px;
    font-weight: 500;
  }
  .beb-col .sub {
    font-size: 11px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 28px;
  }
  .beb-col ul { list-style: none; }
  .beb-col ul li {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    padding: 14px 0;
    border-bottom: 1px dotted var(--rule);
    font-size: 15px;
    color: var(--ink-soft);
  }
  .beb-col ul li.included {
    font-family: 'Cormorant Garamond', serif;
    font-size: 19px;
    color: var(--moss);
    font-weight: 500;
  }
  .beb-col ul li.included::after {
    content: 'Incluso';
    font-family: 'Inter', sans-serif;
    font-size: 10px;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    color: var(--gold);
    font-weight: 500;
  }
  .beb-col ul li .price {
    font-family: 'Cormorant Garamond', serif;
    font-size: 22px;
    color: var(--moss);
    font-weight: 500;
  }
  .beb-col .nota {
    margin-top: 22px;
    font-size: 13px;
    color: var(--muted);
    font-style: italic;
  }

  /* ===== Valores ===== */
  .valores {
    padding: 130px 0;
    background: var(--paper);
    border-top: 1px solid var(--line);
    border-bottom: 1px solid var(--line);
  }
  .precos {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 24px;
    max-width: 1000px;
    margin: 0 auto;
  }
  .preco-card {
    background: var(--cream);
    border: 1px solid var(--line);
    padding: 50px 36px 44px;
    text-align: center;
    position: relative;
    transition: all .3s ease;
  }
  .preco-card.featured {
    background: var(--moss);
    border-color: var(--moss);
    color: var(--cream);
    transform: scale(1.04);
    box-shadow: 0 30px 60px -30px rgba(31,42,33,0.5);
  }
  .preco-card .duracao {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 22px;
    color: var(--gold);
    margin-bottom: 8px;
  }
  .preco-card.featured .duracao { color: var(--gold-soft); }
  .preco-card .label {
    font-size: 10px;
    letter-spacing: 0.4em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 28px;
  }
  .preco-card.featured .label { color: rgba(244,238,226,0.6); }
  .preco-card .valor {
    font-family: 'Cormorant Garamond', serif;
    font-size: 56px;
    font-weight: 400;
    color: var(--moss);
    line-height: 1;
    margin-bottom: 6px;
    letter-spacing: -0.01em;
  }
  .preco-card.featured .valor { color: var(--cream); }
  .preco-card .valor .currency {
    font-size: 22px;
    vertical-align: top;
    margin-right: 2px;
    color: var(--gold);
  }
  .preco-card.featured .valor .currency { color: var(--gold-soft); }
  .preco-card .por {
    font-size: 11px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--muted);
  }
  .preco-card.featured .por { color: rgba(244,238,226,0.6); }
  .preco-card .badge {
    position: absolute;
    top: -12px;
    left: 50%;
    transform: translateX(-50%);
    background: var(--gold);
    color: var(--cream);
    font-size: 9px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    padding: 6px 16px;
    font-weight: 500;
  }
  .precos-foot {
    text-align: center;
    margin-top: 36px;
    font-size: 13px;
    color: var(--muted);
    font-style: italic;
  }

  /* ===== Tabela de preços (valores) ===== */
  .precos-tabela {
    max-width: 880px;
    margin: 0 auto;
    border: 1px solid var(--line);
    background: var(--cream);
    overflow: hidden;
  }
  .ptab-row {
    display: grid;
    grid-template-columns: 2fr 1fr 1fr 1fr;
    border-bottom: 1px solid var(--rule);
    align-items: center;
  }
  .ptab-row:last-child { border-bottom: none; }
  .ptab-row.ptab-head {
    background: var(--moss);
    color: var(--cream);
    font-size: 11px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
  }
  .ptab-row.ptab-head .ptab-cel {
    padding: 16px 24px;
    font-family: 'Inter', sans-serif;
    font-size: 11px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--cream);
    font-weight: 500;
  }
  .ptab-cel {
    padding: 24px;
    font-family: 'Cormorant Garamond', serif;
    font-size: 28px;
    color: var(--moss);
    text-align: center;
  }
  .ptab-cel .cur { font-size: 14px; color: var(--gold); margin-right: 2px; vertical-align: top; }
  .ptab-cel.ptab-empty { color: var(--muted); font-size: 22px; }
  .ptab-name {
    text-align: left !important;
    font-size: 24px !important;
    font-weight: 500;
    display: flex;
    align-items: center;
    gap: 14px;
  }
  .ptab-name .dot {
    width: 8px; height: 8px;
    background: var(--gold);
    border-radius: 50%;
    flex-shrink: 0;
  }
  .ptab-name .tag {
    font-family: 'Inter', sans-serif;
    font-size: 9px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--cream);
    background: var(--gold);
    padding: 4px 10px;
    margin-left: 8px;
  }
  .ptab-row.featured {
    background: var(--paper);
  }
  .ptab-row.featured .ptab-name .dot { background: var(--moss); }
  @media (max-width: 700px) {
    .ptab-row { grid-template-columns: 1fr 1fr; }
    .ptab-row.ptab-head .ptab-cel:first-child { grid-column: 1 / -1; }
    .ptab-name { font-size: 18px !important; padding: 16px 20px !important; }
    .ptab-cel { padding: 14px; font-size: 20px; }
  }
  .info-grid {
    padding: 110px 0;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 80px;
  }
  .info-col h3 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 38px;
    font-weight: 400;
    color: var(--moss);
    margin-bottom: 8px;
  }
  .info-col h3 em { font-style: italic; color: var(--gold); font-weight: 300; }
  .info-col .kicker {
    font-size: 11px;
    letter-spacing: 0.4em;
    text-transform: uppercase;
    color: var(--gold);
    margin-bottom: 12px;
  }
  .info-col ul { list-style: none; margin-top: 28px; }
  .info-col ul li {
    padding: 16px 0;
    border-bottom: 1px solid var(--rule);
    display: flex;
    align-items: baseline;
    gap: 14px;
    color: var(--ink-soft);
    font-size: 15px;
  }
  .info-col ul li::before {
    content: '';
    width: 6px; height: 6px;
    background: var(--gold);
    border-radius: 50%;
    flex-shrink: 0;
    transform: translateY(-2px);
  }
  .beneficios-card {
    background: linear-gradient(180deg, var(--paper), var(--cream-deep));
    padding: 40px;
    border-left: 2px solid var(--gold);
  }
  .beneficios-card .item {
    padding: 16px 0;
    border-bottom: 1px solid var(--rule);
    display: flex;
    align-items: center;
    gap: 16px;
  }
  .beneficios-card .item:last-child { border-bottom: none; }
  .beneficios-card .item .icon {
    width: 36px; height: 36px;
    flex-shrink: 0;
    color: var(--gold);
  }
  .beneficios-card .item .text strong {
    display: block;
    font-family: 'Cormorant Garamond', serif;
    font-size: 22px;
    color: var(--moss);
    font-weight: 500;
    line-height: 1.2;
  }
  .beneficios-card .item .text span {
    font-size: 12px;
    color: var(--muted);
    letter-spacing: 0.05em;
  }

  .obs-row {
    margin-top: 24px;
    padding: 18px 22px;
    background: rgba(168,139,76,0.08);
    border-left: 2px solid var(--gold);
    font-size: 13px;
    line-height: 1.6;
    color: var(--ink-soft);
  }
  .obs-row strong { color: var(--moss); font-weight: 500; }

  /* ===== Condições ===== */
  .condicoes {
    padding: 100px 0;
    background: var(--cream-deep);
  }
  .condicoes-list {
    columns: 2;
    column-gap: 60px;
    list-style: none;
    margin-top: 50px;
  }
  .condicoes-list li {
    break-inside: avoid;
    padding: 14px 0 14px 26px;
    border-bottom: 1px solid var(--rule);
    font-size: 14px;
    color: var(--ink-soft);
    line-height: 1.5;
    position: relative;
  }
  .condicoes-list li::before {
    content: '';
    position: absolute;
    left: 0; top: 22px;
    width: 14px; height: 1px;
    background: var(--gold);
  }

  /* ===== CTA Final ===== */
  .cta {
    background: var(--moss);
    color: var(--cream);
    padding: 140px 0;
    text-align: center;
    position: relative;
    overflow: hidden;
  }
  .cta-bg {
    position: absolute;
    inset: 0;
    opacity: 0.18;
    background: url('assets/salao-bolo.jpg') center/cover;
    filter: blur(2px);
  }
  .cta::after {
    content: '';
    position: absolute;
    inset: 0;
    background: linear-gradient(180deg, rgba(31,42,33,0.85), rgba(31,42,33,0.95));
  }
  .cta-inner { position: relative; z-index: 2; }
  .cta .kicker {
    font-size: 11px;
    letter-spacing: 0.45em;
    text-transform: uppercase;
    color: var(--gold-soft);
    margin-bottom: 28px;
  }
  .cta h2 {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 400;
    font-size: clamp(48px, 6vw, 80px);
    line-height: 1.05;
    color: var(--cream);
    max-width: 800px;
    margin: 0 auto 40px;
  }
  .cta h2 em { font-style: italic; color: var(--gold-soft); }
  .cta .sub {
    color: rgba(244,238,226,0.7);
    max-width: 540px;
    margin: 0 auto 56px;
    font-size: 17px;
  }
  .cta-actions {
    display: flex;
    gap: 18px;
    justify-content: center;
    flex-wrap: wrap;
  }
  .btn {
    display: inline-flex;
    align-items: center;
    gap: 14px;
    padding: 20px 36px;
    font-family: 'Inter', sans-serif;
    font-size: 12px;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    text-decoration: none;
    transition: all .3s ease;
    cursor: pointer;
    border: none;
  }
  .btn-primary {
    background: var(--gold);
    color: var(--cream);
  }
  .btn-primary:hover { background: var(--gold-soft); }
  .btn-ghost {
    background: transparent;
    color: var(--cream);
    border: 1px solid rgba(244,238,226,0.3);
  }
  .btn-ghost:hover { border-color: var(--gold-soft); color: var(--gold-soft); }

  .contato-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 40px;
    margin-top: 80px;
    padding-top: 60px;
    border-top: 1px solid rgba(201,178,122,0.2);
    max-width: 800px;
    margin-left: auto;
    margin-right: auto;
  }
  .contato-grid .item .lbl {
    font-size: 10px;
    letter-spacing: 0.4em;
    text-transform: uppercase;
    color: var(--gold-soft);
    margin-bottom: 10px;
  }
  .contato-grid .item .val {
    font-family: 'Cormorant Garamond', serif;
    font-size: 18px;
    color: var(--cream);
  }

  /* ===== Footer ===== */
  footer {
    background: #14191A;
    color: rgba(244,238,226,0.5);
    padding: 40px 0;
    font-size: 12px;
    text-align: center;
    letter-spacing: 0.1em;
  }

  /* ===== Decorative ornament ===== */
  .ornament {
    text-align: center;
    margin: 60px 0 0;
    color: var(--gold);
    letter-spacing: 1em;
    font-size: 14px;
  }

  /* ===== Responsive ===== */
  @media (max-width: 900px) {
    .container, .topbar-inner { padding-left: 28px; padding-right: 28px; }
    .container-narrow { padding-left: 28px; padding-right: 28px; }
    .topbar nav { display: none; }
    .hero-grid { grid-template-columns: 1fr; gap: 50px; }
    .hero { padding: 70px 0 60px; }
    .saloes { grid-template-columns: 1fr; gap: 32px; }
    .menu-list { columns: 1; }
    .pratos { grid-template-columns: 1fr; gap: 40px; }
    .acomp-grid { grid-template-columns: 1fr 1fr; }
    .beb-grid { grid-template-columns: 1fr; gap: 50px; }
    .precos { grid-template-columns: 1fr; }
    .preco-card.featured { transform: none; }
    .info-grid { grid-template-columns: 1fr; gap: 60px; padding: 70px 0; }
    .condicoes-list { columns: 1; }
    .contato-grid { grid-template-columns: 1fr; gap: 24px; }
    .realizamos .list { font-size: 20px; }
    .realizamos .list span { padding: 4px 14px; }
    .cardapio { padding: 80px 0; }
    .bebidas, .valores { padding: 80px 0; }
  }

  /* ========================================================== */
  /* ============  ESTILOS PARA IMPRESSÃO / PDF  ============== */
  /* ========================================================== */
  @media print {
    @page {
      size: A4 portrait;
      margin: 14mm 12mm;
    }

    * {
      -webkit-print-color-adjust: exact !important;
      print-color-adjust: exact !important;
      color-adjust: exact !important;
    }

    html, body {
      background: var(--cream) !important;
      font-size: 11.5px;
    }

    /* Esconde elementos não úteis em PDF */
    .topbar { display: none !important; }
    body::before { display: none !important; }

    /* Remove animações / transições */
    *, *::before, *::after {
      animation: none !important;
      transition: none !important;
    }

    /* Container mais estreito para A4 */
    .container, .topbar-inner, .container-narrow {
      max-width: 100% !important;
      padding-left: 0 !important;
      padding-right: 0 !important;
    }

    /* Reduz padding vertical das seções */
    .hero { padding: 20px 0 30px !important; }
    .sobre { padding: 30px 0 !important; }
    .galeria { padding: 30px 0 !important; }
    .cardapio { padding: 40px 0 30px !important; }
    .opcional-destaque { padding: 30px 0 !important; }
    .bebidas, .valores { padding: 30px 0 !important; }
    .condicoes { padding: 30px 0 !important; }
    .cta { padding: 30px 0 !important; }

    /* Quebras de página entre seções principais */
    .galeria,
    .cardapio,
    .opcional-destaque,
    .bebidas,
    .valores,
    .condicoes,
    .cta {
      break-before: page;
      page-break-before: always;
    }
    .sobre { break-before: auto; page-break-before: auto; }

    /* Cada pacote em sua própria página */
    .pacote-panel {
      break-before: page;
      page-break-before: always;
      break-inside: avoid;
    }
    .pacote-panel:first-of-type {
      break-before: auto;
      page-break-before: auto;
    }

    /* Evita quebras feias dentro de blocos compactos */
    .menu-block,
    .menu-block-head,
    .ilha-block,
    .prato-grupo,
    .acomp-card,
    .salao-card,
    .preco-card,
    .beb-col,
    .ptab-row,
    .op-card,
    .gimg,
    .condicoes-list li,
    .info-col,
    .obs-row {
      break-inside: avoid;
      page-break-inside: avoid;
    }

    /* Garante fundo do cardápio escuro */
    .cardapio {
      background: var(--moss) !important;
      color: var(--cream) !important;
    }

    /* Ajustes de tipografia para PDF */
    .hero h1,
    .section-head h2 {
      font-size: 38px !important;
      line-height: 1.05 !important;
    }
    .pacote-header .titulo .nome {
      font-size: 36px !important;
    }
    .pacote-header .pp .v { font-size: 28px !important; }
    .menu-block-head h3 { font-size: 24px !important; }
    .op-title { font-size: 36px !important; }
    .op-meta-v { font-size: 30px !important; }

    /* Mosaico da galeria mais compacto no print */
    .galeria-mosaic {
      grid-auto-rows: 48px !important;
      gap: 8px !important;
    }
    .galeria { break-inside: auto; }

    /* CTA final */
    .cta-bg { opacity: 0.10 !important; }

    /* Links sem decoração estranha */
    a { text-decoration: none !important; color: inherit !important; }

    /* Hover states off */
    .gimg:hover img,
    .op-card:hover .op-image img {
      transform: none !important;
      filter: none !important;
    }
  }
</style>
<meta id="dcngeagmmhegagicpcmpinaoklddcgon"></head>
<body>

<!-- ==================== TOPBAR ==================== -->
<header class="topbar">
  <div class="topbar-inner">
    <div class="brand-mark">
      <span class="logo">NAU</span>
      <span class="tag">Eventos · Brasília</span>
    </div>
    <nav>
      <a href="https://019dd5ea-429d-79d8-b3af-5e81b4bc108a.claudeusercontent.com/v1/design/projects/019dd5ea-429d-79d8-b3af-5e81b4bc108a/serve/Proposta%20NAU%20Eventos-print.html?t=2ff205f095966cf5c45810af1caee1654735b6f038dfc39745d99792eed077c6.240c5697-1d2e-4d33-b9a8-3112ae0c9233.50d66e69-32a2-472f-b63b-2a3a81e01ec3.1778716111&amp;direct=1#espacos">Espaços</a>
      <a href="https://019dd5ea-429d-79d8-b3af-5e81b4bc108a.claudeusercontent.com/v1/design/projects/019dd5ea-429d-79d8-b3af-5e81b4bc108a/serve/Proposta%20NAU%20Eventos-print.html?t=2ff205f095966cf5c45810af1caee1654735b6f038dfc39745d99792eed077c6.240c5697-1d2e-4d33-b9a8-3112ae0c9233.50d66e69-32a2-472f-b63b-2a3a81e01ec3.1778716111&amp;direct=1#galeria">Galeria</a>
      <a href="https://019dd5ea-429d-79d8-b3af-5e81b4bc108a.claudeusercontent.com/v1/design/projects/019dd5ea-429d-79d8-b3af-5e81b4bc108a/serve/Proposta%20NAU%20Eventos-print.html?t=2ff205f095966cf5c45810af1caee1654735b6f038dfc39745d99792eed077c6.240c5697-1d2e-4d33-b9a8-3112ae0c9233.50d66e69-32a2-472f-b63b-2a3a81e01ec3.1778716111&amp;direct=1#cardapio">Cardápio</a>
      <a href="https://019dd5ea-429d-79d8-b3af-5e81b4bc108a.claudeusercontent.com/v1/design/projects/019dd5ea-429d-79d8-b3af-5e81b4bc108a/serve/Proposta%20NAU%20Eventos-print.html?t=2ff205f095966cf5c45810af1caee1654735b6f038dfc39745d99792eed077c6.240c5697-1d2e-4d33-b9a8-3112ae0c9233.50d66e69-32a2-472f-b63b-2a3a81e01ec3.1778716111&amp;direct=1#valores">Valores</a>
      <a href="https://019dd5ea-429d-79d8-b3af-5e81b4bc108a.claudeusercontent.com/v1/design/projects/019dd5ea-429d-79d8-b3af-5e81b4bc108a/serve/Proposta%20NAU%20Eventos-print.html?t=2ff205f095966cf5c45810af1caee1654735b6f038dfc39745d99792eed077c6.240c5697-1d2e-4d33-b9a8-3112ae0c9233.50d66e69-32a2-472f-b63b-2a3a81e01ec3.1778716111&amp;direct=1#visita">Agende</a>
    </nav>
  </div>
</header>

<!-- ==================== HERO ==================== -->
<section class="hero">
  <div class="container">
    <div class="hero-grid">
      <div>
        <div class="hero-eyebrow">Proposta · Brasília · 2026</div>
        <h1>Celebrar é<br>o que torna o tempo<br><em>memorável.</em></h1>
        <p class="lead">Na orla da Ponte JK, o NAU recebe casamentos, aniversários e celebrações com cardápio premiado, ambiente diferenciado e estacionamento exclusivo. Esta é a nossa proposta para o seu próximo momento especial.</p>
        <div class="ornament">✦ ✦ ✦</div>
      </div>
      <div class="hero-image">
        <img src="./NAU Eventos · Proposta_files/hero-cerimonia.jpeg" alt="Cerimônia no NAU com teto de orquídeas brancas e decoração de casamento ao anoitecer">
        <div class="caption">Cerimônia · teto de orquídeas</div>
      </div>
    </div>
  </div>
</section>

<!-- ==================== SOBRE + SALÕES ==================== -->
<section class="sobre" id="espacos">
  <div class="container">
    <div class="section-head">
      <div class="kicker">Sobre o NAU</div>
      <h2>Um endereço pensado<br>para <em>momentos raros.</em></h2>
    </div>

    <div class="sobre-intro">
      <p>Localizado em uma das regiões mais nobres de Brasília, o NAU oferece tudo que o seu evento precisa: ambiente diferenciado, cardápio premiado, espaços para cerimônia e estacionamento exclusivo e gratuito.</p>
    </div>

    <div class="saloes">
      <div class="salao-card">
        <div class="image">
          <img src="./NAU Eventos · Proposta_files/salao-jantar.jpg" alt="Salão JK do NAU montado para jantar com flores brancas e iluminação intimista">
        </div>
        <div class="body">
          <div class="number">i.</div>
          <h3>Salão JK</h3>
          <p>Configuração única com área climatizada, varanda e deck exclusivo com vista para a Ponte JK. Ideal para celebrações intimistas que pedem a paisagem mais bonita da cidade.</p>
          <div class="salao-meta">
            <div class="item">
              <div class="label">Capacidade</div>
              <div class="value">120 <small>pessoas</small></div>
            </div>
            <div class="item">
              <div class="label">A partir de</div>
              <div class="value">40 <small>pessoas</small></div>
            </div>
          </div>
        </div>
      </div>

      <div class="salao-card">
        <div class="image">
          <img src="./NAU Eventos · Proposta_files/salao-lounge.jpg" alt="Lounge do Salão do Porto com sofás e flores">
        </div>
        <div class="body">
          <div class="number">ii.</div>
          <h3>Salão do Porto</h3>
          <p>Espaço amplo, reservado e com entrada exclusiva. Comporta montagem de show e pista de dança — perfeito para festas com energia, música ao vivo e muitos convidados.</p>
          <div class="salao-meta">
            <div class="item">
              <div class="label">Capacidade</div>
              <div class="value">190 <small>pessoas</small></div>
            </div>
            <div class="item">
              <div class="label">A partir de</div>
              <div class="value">60 <small>pessoas</small></div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="realizamos">
      <div class="label">Realizamos</div>
      <div class="list">
        <span>Casamentos</span>
        <span>Aniversários</span>
        <span>Batizados</span>
        <span>Festas Infantis</span>
        <span>Eventos Corporativos</span>
      </div>
    </div>
  </div>
</section>

<!-- ==================== GALERIA · MOMENTOS NAU ==================== -->
<section class="galeria" id="galeria">
  <div class="container">
    <div class="section-head">
      <div class="kicker">Momentos NAU</div>
      <h2>Cada evento,<br>uma <em>história única.</em></h2>
      <p>Um recorte de cerimônias, jantares e celebrações que aconteceram no NAU — para você imaginar a sua.</p>
    </div>

    <div class="galeria-meta">
      <span>Cerimônias</span>
      <span>Jantares</span>
      <span>Decoração</span>
      <span>Bar &amp; Doces</span>
    </div>

    <div class="galeria-mosaic">
      <figure class="gimg g1">
        <span class="gnum">i.</span>
        <img src="./NAU Eventos · Proposta_files/galeria-01.jpeg" alt="Mesa de jantar com louça verde, taças de cristal e arranjo central de rosas brancas">
        <figcaption class="gcap">Mesa posta — louça verde e rosas brancas</figcaption>
      </figure>

      <figure class="gimg g2">
        <span class="gnum">ii.</span>
        <img src="./NAU Eventos · Proposta_files/galeria-02.jpeg" alt="Cerimônia com arco circular de flores brancas e corredor de chuva-de-prata">
        <figcaption class="gcap">Arco de flores brancas · cerimônia</figcaption>
      </figure>

      <figure class="gimg g3">
        <span class="gnum">iii.</span>
        <img src="./NAU Eventos · Proposta_files/galeria-03.jpeg" alt="Altar ao ar livre com vista para a ponte JK e tapete de chuva-de-prata">
        <figcaption class="gcap">Altar com vista — ponte JK</figcaption>
      </figure>

      <figure class="gimg g4">
        <span class="gnum">iv.</span>
        <img src="./NAU Eventos · Proposta_files/galeria-04.jpeg" alt="Mesa de bolo com arranjos florais em tons de roxo e iluminação cênica">
        <figcaption class="gcap">Mesa de bolo · paleta lilás</figcaption>
      </figure>

      <figure class="gimg g5">
        <span class="gnum">v.</span>
        <img src="./NAU Eventos · Proposta_files/galeria-05.jpg" alt="Cerimônia noturna com teto de orquídeas brancas suspensas e cadeiras de acrílico">
        <figcaption class="gcap">Cerimônia noturna · teto de orquídeas</figcaption>
      </figure>

      <figure class="gimg g6">
        <span class="gnum">vi.</span>
        <img src="./NAU Eventos · Proposta_files/galeria-06.jpg" alt="Bar de drinks com equipe de bartenders uniformizados e arranjos suspensos">
        <figcaption class="gcap">Bar &amp; mixologia autoral</figcaption>
      </figure>

      <figure class="gimg g7">
        <span class="gnum">vii.</span>
        <img src="./NAU Eventos · Proposta_files/galeria-07.jpg" alt="Mesa de doces e bolo de casamento ao entardecer com vista para o lago">
        <figcaption class="gcap">Mesa de doces ao entardecer · vista do lago</figcaption>
      </figure>
    </div>

    <p class="galeria-foot">O cenário você já viu. Agora, escolha o cardápio que vai compor a sua noite.</p>
  </div>
</section>

<!-- ==================== CARDÁPIO PREMIUM ==================== -->
<section class="cardapio" id="cardapio">
  <div class="container">
    <div class="section-head">
      <div class="kicker">Nossos Cardápios</div>
      <h2>Três pacotes,<br><em>três experiências.</em></h2>
      <p>Cada pacote tem o seu próprio cardápio completo e a sua faixa de preços por duração de evento. Role para conhecer todos.</p>
    </div>

    <!-- ==================== PACOTE OURO ==================== -->
    <div class="pacote-panel active" data-pacote="ouro" data-pacote-name="Pacote Ouro">
      <div class="pacote-header">
        <div class="titulo">
          <div class="eyebrow">Pacote</div>
          <div class="nome">Ouro</div>
        </div>
        <div class="precos-row">
          <div class="pp"><div class="h">3 horas</div><div class="v"><span class="c">R$</span>273</div><div class="pp-foot">por pessoa</div></div>
          <div class="pp"><div class="h">4 horas</div><div class="v"><span class="c">R$</span>286</div><div class="pp-foot">por pessoa</div></div>
          <div class="pp"><div class="h">5 horas</div><div class="v"><span class="c">R$</span>299</div><div class="pp-foot">por pessoa</div></div>
        </div>
      </div>
      <p class="pacote-intro">Um menu equilibrado, com sabores marcantes e o cuidado de sempre — perfeito para celebrações que pedem clássicos bem executados.</p>

      <div class="menu-block">
        <div class="menu-block-head">
          <div class="num">i.</div>
          <h3>Entradas Volantes</h3>
          <div class="hint">circulam pelos convidados</div>
        </div>
        <ul class="menu-list">
          <li>Mini pastel 3 queijos</li>
          <li>Crocante de isca de peixe com molho Navete</li>
          <li>Ceviche de Saint Peter</li>
          <li>Dadinho de tapioca com mel de rapadura</li>
          <li>Chips de batata doce com creme de parmesão</li>
          <li>Cestinha de massa filo com frango e requeijão</li>
          <li>Bobó de peixe com camarão</li>
          <li>Crostini de abobrinha e berinjela com calda de laranja</li>
        </ul>
      </div>

      <div class="menu-block">
        <div class="menu-block-head">
          <div class="num">ii.</div>
          <h3>Pratos Principais</h3>
          <div class="hint">servidos com cuidado · serviço buffet</div>
        </div>
        <div class="pratos">
          <div class="prato-grupo">
            <div class="gp-head"><h4>Camarão</h4><div class="pick">escolha 1</div></div>
            <ul>
              <li>
                <div class="nome">Camarão NAU</div>
                <div class="desc">Camarões refogados na manteiga aromatizada, servidos envolto em arroz cremoso de manjericão, gratinado com queijo muçarela.</div>
              </li>
              <li>
                <div class="nome">Camarão Poldina</div>
                <div class="desc">Camarões refogados na manteiga aromatizada, servidos envolto em arroz cremoso de nata, queijo coalho e salsinha, coberto com cubinhos de queijo coalho empanados.</div>
              </li>
            </ul>
          </div>
          <div class="prato-grupo">
            <div class="gp-head"><h4>Peixe</h4><div class="pick">escolha 1</div></div>
            <ul>
              <li>
                <div class="nome">Filé de Tilápia Crocante</div>
                <div class="desc">Em crosta de parmesão, panko e toque suave de limão siciliano.</div>
              </li>
              <li>
                <div class="nome">Filé de Tilápia ao Molho de Ervas Finas</div>
                <div class="desc">Finalizado com ervas frescas e manteiga clarificada.</div>
              </li>
              <li>
                <div class="nome">Peixe com Tomatinhos</div>
                <div class="desc">Salteado no azeite com tomatinhos e manjericão fresco.</div>
              </li>
            </ul>
          </div>
          <div class="prato-grupo">
            <div class="gp-head"><h4>Carne</h4><div class="pick">escolha 1</div></div>
            <ul>
              <li>
                <div class="nome">Medalhão de Alcatra</div>
                <div class="desc">Com molho de queijo gorgonzola e cebolinha.</div>
              </li>
              <li>
                <div class="nome">Maminha</div>
                <div class="desc">Com pétalas de cebola caramelizada e bacon.</div>
              </li>
            </ul>
          </div>
        </div>

        <div class="acomp-grid">
          <div class="acomp-card">
            <h5>Acompanhamentos</h5>
            <div class="pick">escolha 3</div>
            <ul>
              <li>Arroz com brócolis</li>
              <li>Arroz branco</li>
              <li>Ratatouille de legumes</li>
              <li>Legumes no vapor</li>
              <li>Batata ao forno com ervas finas</li>
            </ul>
          </div>
          <div class="acomp-card">
            <h5>Fettuccine</h5>
            <div class="pick">escolha 2 molhos</div>
            <ul>
              <li>Pesto com castanhas</li>
              <li>Pomodoro</li>
              <li>04 queijos</li>
              <li>Bechamel com cogumelos frescos</li>
            </ul>
          </div>
          <div class="acomp-card">
            <h5>Salada</h5>
            <div class="pick">escolha 1</div>
            <ul>
              <li>Salada tropical · 3 folhas verdes, tomate cereja e frutas da estação</li>
              <li>Salada Caesar · clássica</li>
            </ul>
          </div>
          <div class="acomp-card">
            <h5>Bebidas Inclusas</h5>
            <div class="pick">à vontade</div>
            <ul>
              <li>Água c/ e s/ gás</li>
              <li>Coca-Cola normal e zero</li>
              <li>Guaraná normal e zero</li>
              <li>Café expresso</li>
              <li>Sucos naturais · laranja, abacaxi com hortelã</li>
            </ul>
          </div>
        </div>
      </div>

      <div class="menu-block ilha-block">
        <div class="menu-block-head">
          <div class="num">iii.</div>
          <h3>Ilha Gourmet <span class="opt-badge">opcional</span></h3>
          <div class="hint">serviço à parte · <strong class="ilha-price">+ R$ 40</strong> por pessoa</div>
        </div>
        <ul class="menu-list">
          <li>Pães artesanais, grissini e focaccia</li>
          <li>Chips de batata doce</li>
          <li>Guacamole</li>
          <li>Queijo parmesão</li>
          <li>Queijo provolone</li>
          <li>Queijo brie</li>
          <li>Queijo marinado com azeite, ervas e azeitonas</li>
          <li>Lâminas de blanquet de peru</li>
          <li>Lâminas de salaminho</li>
          <li>Geleia de morango</li>
          <li>Chutney de abacaxi com pimenta</li>
          <li>Pasta de tomate seco</li>
          <li>Terrine de queijo e cebola caramelizada</li>
          <li>Tomatinho caprese</li>
        </ul>
      </div>
    </div>

    <!-- ==================== PACOTE PREMIUM ==================== -->
    <div class="pacote-panel" data-pacote="premium" data-pacote-name="Pacote Premium">
      <div class="pacote-header">
        <div class="titulo">
          <div class="eyebrow">Pacote · Mais escolhido</div>
          <div class="nome">Premium</div>
        </div>
        <div class="precos-row">
          <div class="pp"><div class="h">3 horas</div><div class="v"><span class="c">R$</span>286</div><div class="pp-foot">por pessoa</div></div>
          <div class="pp"><div class="h">4 horas</div><div class="v"><span class="c">R$</span>305</div><div class="pp-foot">por pessoa</div></div>
          <div class="pp"><div class="h">5 horas</div><div class="v"><span class="c">R$</span>337</div><div class="pp-foot">por pessoa</div></div>
        </div>
      </div>
      <p class="pacote-intro">O cardápio mais escolhido da casa — entradas variadas, três opções de carne, peixe e camarão, e finalização generosa.</p>

      <div class="menu-block">
        <div class="menu-block-head">
          <div class="num">i.</div>
          <h3>Entradas Volantes</h3>
          <div class="hint">circulam pelos convidados</div>
        </div>
        <ul class="menu-list">
          <li>Croquete de costela na panko</li>
          <li>Dadinho de tapioca com melaço de cana</li>
          <li>Ceviche de peixe</li>
          <li>Espetada de camarão empanado</li>
          <li>Arrozinho de ossobuco com crisp de cebola</li>
          <li>Folhado de creme de queijo com tomate seco e manjericão</li>
          <li>Bolinho crocante de salmão</li>
          <li>Crocante de isca de peixe com molho Navete</li>
        </ul>
      </div>

      <div class="menu-block">
        <div class="menu-block-head">
          <div class="num">ii.</div>
          <h3>Pratos Principais</h3>
          <div class="hint">servidos com cuidado · serviço buffet</div>
        </div>
        <div class="pratos">
          <div class="prato-grupo">
            <div class="gp-head"><h4>Camarão</h4><div class="pick">escolha 1</div></div>
            <ul>
              <li>
                <div class="nome">Camarão Fortuna do Mar</div>
                <div class="desc">Camarões refogados na manteiga aromatizada com tomate seco, palmito, cebola, azeitonas verdes e roxas (com caroço), servidos sobre arroz cremoso de tomate seco.</div>
              </li>
              <li>
                <div class="nome">Camarão Sofisticado</div>
                <div class="desc">Camarões salteados na manteiga com arroz cremoso de nata e mostarda, pedacinhos de palmito e cubos de queijo coalho.</div>
              </li>
              <li>
                <div class="nome">Camarão Laguna</div>
                <div class="desc">Camarões salteados na manteiga envolto em arroz cremoso de queijo catupiry e pedacinhos de damasco.</div>
              </li>
            </ul>
          </div>
          <div class="prato-grupo">
            <div class="gp-head"><h4>Peixe</h4><div class="pick">escolha 1</div></div>
            <ul>
              <li><div class="nome">Salmão na Chapa</div><div class="desc">Com molho de maracujá e farofa crocante.</div></li>
              <li><div class="nome">Peixe Aromatizado</div><div class="desc">Manteiga de sálvia e castanhas de caju.</div></li>
              <li><div class="nome">Filé de Dourado</div><div class="desc">No crocante de panko e ervas finas.</div></li>
            </ul>
          </div>
          <div class="prato-grupo">
            <div class="gp-head"><h4>Carne</h4><div class="pick">escolha 1</div></div>
            <ul>
              <li><div class="nome">Escalopinho de Filé Mignon</div><div class="desc">Ao molho de vinho tinto com cubinhos de bacon e cebola crisp.</div></li>
              <li><div class="nome">Filé Barlavento</div><div class="desc">Receita da casa.</div></li>
              <li><div class="nome">Cubos de Filé Convés</div><div class="desc">Salteados no azeite com molho convés.</div></li>
            </ul>
          </div>
        </div>

        <div class="acomp-grid">
          <div class="acomp-card">
            <h5>Acompanhamentos</h5>
            <div class="pick">escolha 3</div>
            <ul>
              <li>Arroz com brócolis</li>
              <li>Arroz branco</li>
              <li>Arroz 7 grãos</li>
              <li>Ratatouille de legumes</li>
              <li>Legumes no vapor</li>
              <li>Batata ao forno com ervas finas</li>
            </ul>
          </div>
          <div class="acomp-card">
            <h5>Fettuccine</h5>
            <div class="pick">escolha 2 molhos</div>
            <ul>
              <li>Pesto com castanhas</li>
              <li>Pomodoro</li>
              <li>04 queijos</li>
              <li>Bechamel com cogumelos frescos</li>
            </ul>
          </div>
          <div class="acomp-card">
            <h5>Salada</h5>
            <div class="pick">escolha 1</div>
            <ul>
              <li>Salada tropical · 3 folhas verdes, tomate cereja e frutas da estação</li>
              <li>Salada Farol · rúcula, alface americana, queijo branco, tomate seco, tomate cereja, castanha e torradas crocantes — aceto balsâmico, shoyu e azeite</li>
              <li>Salada fria de abobrinha e berinjela com queijo minas, tomate seco e manjericão</li>
            </ul>
          </div>
          <div class="acomp-card">
            <h5>Bebidas Inclusas</h5>
            <div class="pick">à vontade</div>
            <ul>
              <li>Água c/ e s/ gás</li>
              <li>Coca-Cola normal e zero</li>
              <li>Guaraná normal e zero</li>
              <li>Café expresso</li>
              <li>Sucos naturais · laranja, abacaxi com hortelã</li>
            </ul>
          </div>
        </div>
      </div>

      <div class="menu-block ilha-block">
        <div class="menu-block-head">
          <div class="num">iii.</div>
          <h3>Ilha Gourmet <span class="opt-badge">opcional</span></h3>
          <div class="hint">serviço à parte · <strong class="ilha-price">+ R$ 60</strong> por pessoa</div>
        </div>
        <ul class="menu-list">
          <li>Pães artesanais, grissini e focaccia</li>
          <li>Chips de batata doce</li>
          <li>Guacamole</li>
          <li>Queijo parmesão</li>
          <li>Queijo provolone</li>
          <li>Queijo brie</li>
          <li>Queijo marinado com azeite, ervas e azeitonas</li>
          <li>Lâminas de blanquet de peru</li>
          <li>Lâminas de salaminho</li>
          <li>Geleia de morango</li>
          <li>Chutney de abacaxi com pimenta</li>
          <li>Pasta de tomate seco</li>
          <li>Terrine de queijo com gorgonzola</li>
          <li>Salada de tomatinhos caprese</li>
          <li>Quiche de alho-poró e bacalhau</li>
        </ul>
      </div>
    </div>

    <!-- ==================== MENU TEEN ==================== -->
    <div class="pacote-panel" data-pacote="teen" data-pacote-name="Menu Teen">
      <div class="pacote-header">
        <div class="titulo">
          <div class="eyebrow">Menu · Festa jovem</div>
          <div class="nome">Teen</div>
        </div>
        <div class="precos-row">
          <div class="pp"><div class="h">3 horas</div><div class="v"><span class="c">R$</span>273</div><div class="pp-foot">por pessoa</div></div>
          <div class="pp"><div class="h">4 horas</div><div class="v"><span class="c">R$</span>286</div><div class="pp-foot">por pessoa</div></div>
          <div class="pp"><div class="h">5 horas</div><div class="v"><span class="c">R$</span>299</div><div class="pp-foot">por pessoa</div></div>
        </div>
      </div>
      <p class="pacote-intro">Para festas adolescentes e infanto-juvenis — coquetel volante seguido de pratos quentes e sanduíches, na vibe descontraída.</p>

      <div class="menu-block">
        <div class="menu-block-head">
          <div class="num">i.</div>
          <h3>Coquetel Volante</h3>
          <div class="hint">circulam pelos convidados</div>
        </div>
        <ul class="menu-list">
          <li>Pastel de Camarão</li>
          <li>Pastel de Três Queijos</li>
          <li>Coxinha de Frango Gourmet</li>
          <li>Cestinha de Massa Filo com Frango e Requeijão</li>
          <li>Isca de Peixe com Molho Navete</li>
          <li>Croquete de Carne com Molho de Mostarda</li>
          <li>Dadinho de Tapioca com Melaço de Cana</li>
          <li>Folhado de Tomate Seco e Manjericão</li>
          <li>Bobó de Peixe com Camarão</li>
          <li>Crostini de Abobrinha e Berinjela com Calda de Laranja</li>
        </ul>
      </div>

      <div class="menu-block">
        <div class="menu-block-head">
          <div class="num">ii.</div>
          <h3>Pratos Principais</h3>
          <div class="hint">servidos com cuidado · serviço buffet</div>
        </div>
        <div class="pratos">
          <div class="prato-grupo">
            <div class="gp-head"><h4>Camarão</h4><div class="pick">escolha 1</div></div>
            <ul>
              <li>
                <div class="nome">Camarão NAU</div>
                <div class="desc">Camarões refogados na manteiga aromatizada, servidos envolto em arroz cremoso de manjericão, gratinado com queijo muçarela.</div>
              </li>
              <li>
                <div class="nome">Camarão Poldina</div>
                <div class="desc">Camarões refogados na manteiga aromatizada, servidos envolto em arroz cremoso de nata, queijo coalho e salsinha, coberto com cubinhos de queijo coalho empanados.</div>
              </li>
            </ul>
          </div>
          <div class="prato-grupo">
            <div class="gp-head"><h4>Carne</h4><div class="pick">escolha 1</div></div>
            <ul>
              <li>
                <div class="nome">Medalhão de Alcatra</div>
                <div class="desc">Com molho de queijo gorgonzola e cebolinha.</div>
              </li>
              <li>
                <div class="nome">Maminha</div>
                <div class="desc">Com pétalas de cebola caramelizada e bacon.</div>
              </li>
            </ul>
          </div>
          <div class="prato-grupo">
            <div class="gp-head"><h4>Sanduíches</h4><div class="pick">escolha 1</div></div>
            <ul>
              <li>
                <div class="nome">Mini Hambúrgueres Artesanais</div>
                <div class="desc">Pão brioche, blend de carne e queijo derretido.</div>
              </li>
              <li>
                <div class="nome">Sanduíche de Carne de Sol com Nata</div>
                <div class="desc">Pão de fermentação natural, carne de sol e nata.</div>
              </li>
              <li>
                <div class="nome">Mini Hot-Dog</div>
                <div class="desc">Pão de leite, salsicha e batata palha.</div>
              </li>
            </ul>
          </div>
        </div>

        <div class="acomp-grid">
          <div class="acomp-card">
            <h5>Acompanhamentos</h5>
            <div class="pick">escolha 1</div>
            <ul>
              <li>Arroz com brócolis</li>
              <li>Arroz branco</li>
              <li>Ratatouille de legumes</li>
              <li>Legumes no vapor</li>
              <li>Batata ao forno com ervas finas</li>
            </ul>
          </div>
          <div class="acomp-card">
            <h5>Fettuccine</h5>
            <div class="pick">escolha 2 molhos</div>
            <ul>
              <li>Pomodoro</li>
              <li>04 queijos</li>
              <li>Bechamel com cogumelos frescos</li>
            </ul>
          </div>
          <div class="acomp-card">
            <h5>Bebidas Inclusas</h5>
            <div class="pick">à vontade</div>
            <ul>
              <li>Água c/ e s/ gás</li>
              <li>Coca-Cola normal e zero</li>
              <li>Guaraná normal e zero</li>
              <li>Café Expresso</li>
            </ul>
          </div>
          <div class="acomp-card">
            <h5>Sucos Naturais</h5>
            <div class="pick">escolha 2 sabores</div>
            <ul>
              <li>Laranja</li>
              <li>Melancia</li>
              <li>Abacaxi com Hortelã</li>
              <li>Laranja com Morango</li>
            </ul>
          </div>
        </div>
      </div>

      <div class="menu-block ilha-block">
        <div class="menu-block-head">
          <div class="num">iii.</div>
          <h3>Ilha Gourmet <span class="opt-badge">opcional</span></h3>
          <div class="hint">serviço à parte · <strong class="ilha-price">+ R$ 40</strong> por pessoa</div>
        </div>
        <ul class="menu-list">
          <li>Pães artesanais, grissini e focaccia</li>
          <li>Chips de batata doce</li>
          <li>Guacamole</li>
          <li>Queijo parmesão</li>
          <li>Queijo provolone</li>
          <li>Queijo brie</li>
          <li>Queijo marinado com azeite, ervas e azeitonas</li>
          <li>Lâminas de blanquet de peru</li>
          <li>Lâminas de salaminho</li>
          <li>Geleia de morango</li>
          <li>Chutney de abacaxi com pimenta</li>
          <li>Pasta de tomate seco</li>
          <li>Terrine de queijo e cebola caramelizada</li>
          <li>Tomatinho caprese</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- ==================== SERVIÇO OPCIONAL · CARRINHO DE LAGOSTA ==================== -->
<section class="opcional-destaque">
  <div class="container">
    <div class="op-card">
      <div class="op-image">
        <img src="./NAU Eventos · Proposta_files/lagosta-carrinho.png" alt="Carrinho gourmet de lagosta com risoto de limão siciliano servido em tábua de madeira">
        <div class="op-tag">Serviço opcional</div>
      </div>
      <div class="op-body">
        <div class="op-eyebrow">Destaque da casa</div>
        <h3 class="op-title">Carrinho Gourmet<br><em>de Lagosta</em></h3>
        <p class="op-sub">com risoto de limão siciliano · finalização ao vivo em carrinho gourmet montado no salão.</p>

        <div class="op-meta">
          <div class="op-meta-cell">
            <div class="op-meta-h">Investimento</div>
            <div class="op-meta-v"><span class="cur">R$</span>68<span class="unit">/ pessoa</span></div>
          </div>
          <div class="op-meta-cell">
            <div class="op-meta-h">Duração do serviço</div>
            <div class="op-meta-v"><span class="num">1h30</span><span class="unit">durante o evento</span></div>
          </div>
        </div>

        <div class="op-foot">
          Contratação fechada pelo número total de convidados do evento.<br>
          <span class="op-foot-defeso">Sujeito a disponibilidade — período de defeso da lagosta: <strong>1º de novembro a 30 de abril</strong> (Portaria SAP/MAPA nº 215/2020).</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ==================== BEBIDAS OPCIONAIS ==================== -->
<section class="bebidas">
  <div class="container">
    <div class="section-head">
      <div class="kicker">Bebidas opcionais</div>
      <h2>Para quando a noite<br>pede <em>um brinde a mais.</em></h2>
      <p>Adicione bebidas alcoólicas ao seu pacote — preço por pessoa, à vontade durante todo o evento.</p>
    </div>

    <div class="beb-grid">
      <div class="beb-col">
        <h4>Bebidas Inclusas</h4>
        <div class="sub">já fazem parte do pacote</div>
        <ul>
          <li class="included">Refrigerantes Coca-Cola e Guaraná</li>
          <li class="included">Água mineral com e sem gás</li>
          <li class="included">Café Expresso</li>
          <li class="included">Sucos Naturais · laranja, abacaxi com hortelã</li>
        </ul>
      </div>

      <div class="beb-col">
        <h4>Acréscimos Opcionais</h4>
        <div class="sub">por pessoa, à vontade</div>
        <ul>
          <li><span>Cerveja Heineken 600ml</span> <span class="price">R$ 33</span></li>
          <li><span>Caipifrutas de Cachaça <small>· 3 sabores</small></span> <span class="price">R$ 36</span></li>
          <li><span>Caipifrutas de Smirnoff <small>· 3 sabores</small></span> <span class="price">R$ 50</span></li>
          <li><span>Caipifrutas de Absolut <small>· 3 sabores</small></span> <span class="price">R$ 55</span></li>
          <li><span>Vinho Branco e Tinto</span> <span class="price">R$ 58</span></li>
          <li><span>Espumante Brut e Moscatel</span> <span class="price">R$ 66</span></li>
          <li><span>Vinho Tinto + Espumante Brut</span> <span class="price">R$ 66</span></li>
        </ul>
        <div class="nota">Valores por pessoa, durante a duração contratada do evento.</div>
      </div>
    </div>
  </div>
</section>

<!-- ==================== VALORES ==================== -->
<section class="valores" id="valores">
  <div class="container">
    <div class="section-head">
      <div class="kicker">Investimento</div>
      <h2>Três pacotes,<br><em>um só cuidado.</em></h2>
      <p>Valores por pessoa — incluem cardápio completo, bebidas não alcoólicas, espaço, equipe e estrutura. Vigente para eventos de janeiro a dezembro de 2026.</p>
    </div>

    <div class="precos-tabela">
      <div class="ptab-row ptab-head">
        <div class="ptab-cel ptab-name">Pacote</div>
        <div class="ptab-cel">3 horas</div>
        <div class="ptab-cel">4 horas</div>
        <div class="ptab-cel">5 horas</div>
      </div>
      <div class="ptab-row">
        <div class="ptab-cel ptab-name"><span class="dot"></span>Ouro</div>
        <div class="ptab-cel"><span class="cur">R$</span>273</div>
        <div class="ptab-cel"><span class="cur">R$</span>286</div>
        <div class="ptab-cel"><span class="cur">R$</span>299</div>
      </div>
      <div class="ptab-row featured">
        <div class="ptab-cel ptab-name"><span class="dot"></span>Premium <span class="tag">Mais escolhido</span></div>
        <div class="ptab-cel"><span class="cur">R$</span>286</div>
        <div class="ptab-cel"><span class="cur">R$</span>305</div>
        <div class="ptab-cel"><span class="cur">R$</span>337</div>
      </div>
      <div class="ptab-row">
        <div class="ptab-cel ptab-name"><span class="dot"></span>Menu Teen</div>
        <div class="ptab-cel"><span class="cur">R$</span>273</div>
        <div class="ptab-cel"><span class="cur">R$</span>286</div>
        <div class="ptab-cel"><span class="cur">R$</span>299</div>
      </div>
    </div>

    <div class="precos-foot">Valores por pessoa · vigentes para eventos realizados de janeiro a dezembro de 2026.</div>
  </div>
</section>

<!-- ==================== PAGAMENTO + BENEFÍCIOS ==================== -->
<section>
  <div class="container">
    <div class="info-grid">
      <div class="info-col">
        <div class="kicker">Formas de pagamento</div>
        <h3>Pagamento <em>sem complicação.</em></h3>
        <ul>
          <li>Cartão em até <strong>4×</strong> &nbsp;<small style="color:var(--muted);font-size:13px">para valores acima de R$ 5.000</small></li>
          <li>Boleto bancário</li>
          <li>Dinheiro &nbsp;ou&nbsp; PIX</li>
        </ul>
        <div class="obs-row">
          <strong>OBS</strong> · Para eventos com duração maior que a contratada, será cobrada uma taxa de R$ 55,00 por convidado/hora.
        </div>
      </div>

      <div class="info-col">
        <div class="kicker">Benefícios exclusivos</div>
        <h3>Cortesias <em>deste cardápio.</em></h3>
        <div class="beneficios-card">
          <div class="item">
            <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.2"><path d="M8 8 V4 a4 4 0 1 1 8 0 V8"></path><path d="M5 8 h14 v3 a7 7 0 0 1-14 0 z"></path><path d="M12 18 v3"></path><path d="M9 21 h6"></path></svg>
            <div class="text">
              <strong>Taxa de rolha promocional</strong>
              <span>Apenas R$ 30,00 por garrafa</span>
            </div>
          </div>
          <div class="item">
            <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.2"><path d="M3 11 L12 4 L21 11"></path><path d="M5 10 V20 h14 V10"></path><path d="M9 20 V14 h6 V20"></path></svg>
            <div class="text">
              <strong>Locação do espaço · cortesia</strong>
              <span>Não cobramos pela utilização do salão</span>
            </div>
          </div>
          <div class="item">
            <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.2"><rect x="3" y="11" width="18" height="8" rx="1"></rect><path d="M5 11 L7 5 h10 l2 6"></path><circle cx="7.5" cy="19" r="1.5"></circle><circle cx="16.5" cy="19" r="1.5"></circle></svg>
            <div class="text">
              <strong>Estacionamento coberto</strong>
              <span>Exclusivo,coberto e gratuito para os convidados. Mediante disponibilidade de vagas.</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ==================== CONDIÇÕES ==================== -->
<section class="condicoes">
  <div class="container">
    <div class="section-head" style="margin-bottom:20px">
      <div class="kicker">Condições gerais</div>
      <h2 style="font-size:clamp(36px,4vw,48px)">Para alinharmos <em>cada detalhe.</em></h2>
    </div>

    <ul class="condicoes-list">
      <li>Espaço exclusivo durante todo o evento.</li>
      <li>Serviço de buffet disponível para grupos a partir de 50 pessoas.</li>
      <li>Trabalhamos com no-show: caso compareça um número inferior, será considerado o número contratado; se compareça maior, será considerado o número real.</li>
      <li>Não há ressarcimento de valores caso compareça um número inferior ao contratado.</li>
      <li>Mediante interesse, o cliente terá acesso ao Contrato de Prestação de Serviço.</li>
      <li>Este orçamento <strong>não garante a reserva</strong> da data e do horário.</li>
      <li>Não trabalhamos com equipamento de áudio e vídeo.</li>
      <li>Para eventos com duração maior, verificar o preço da hora adicional.</li>
      <li>Para uso de som, verificar condições.</li>
      <li>A decoração do espaço não é de nossa responsabilidade.</li>
      <li>Obrigatório o uso de gerador de energia.</li>
    </ul>
  </div>
</section>

<!-- ==================== CTA FINAL ==================== -->
<section class="cta" id="visita">
  <div class="cta-bg"></div>
  <div class="container cta-inner">
    <div class="kicker">Próximo passo</div>
    <h2>Vamos <em>conhecer o NAU</em><br>juntos?</h2>
    <p class="sub">Agende uma visita com nossa equipe e veja de perto os salões, os pratos e o espaço onde o seu evento pode acontecer.</p>

    <div class="cta-actions">
      <a class="btn btn-primary" href="https://wa.me/5561995590001" target="_blank" rel="noopener">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M17.5 14.4c-.3-.1-1.7-.8-2-.9-.3-.1-.5-.2-.7.1-.2.3-.8.9-1 1.1-.2.2-.4.2-.6.1-.3-.1-1.2-.4-2.3-1.4-.9-.8-1.4-1.7-1.6-2-.2-.3 0-.5.1-.6.1-.1.3-.4.4-.5.1-.2.2-.3.2-.5 0-.2 0-.3-.1-.4 0-.1-.7-1.6-.9-2.2-.2-.6-.5-.5-.7-.5h-.6c-.2 0-.5.1-.7.4-.2.3-.9.9-.9 2.2 0 1.3.9 2.5 1 2.7.1.2 1.8 2.7 4.4 3.8.6.3 1.1.4 1.5.5.6.2 1.2.2 1.6.1.5-.1 1.7-.7 1.9-1.4.2-.7.2-1.2.2-1.4-.1-.2-.3-.3-.6-.4zM12 22c-1.7 0-3.4-.5-4.9-1.3l-3.4 1 1-3.3C3.7 16.7 3 14.4 3 12 3 7 7 3 12 3s9 4 9 9-4 10-9 10z"></path></svg>
        Conversar no WhatsApp
      </a>
      <a class="btn btn-ghost" href="mailto:eventosdf@naufrutosdomar.com.br">
        Enviar e-mail
      </a>
    </div>

    <div class="contato-grid">
      <div class="item">
        <div class="lbl">Equipe</div>
        <div class="val">NAU Eventos</div>
      </div>
      <div class="item">
        <div class="lbl">Telefone</div>
        <div class="val">(61) 99559.0001</div>
      </div>
      <div class="item">
        <div class="lbl">E-mail</div>
        <div class="val">eventosdf@naufrutosdomar.com.br</div>
      </div>
    </div>
  </div>
</section>

<footer>
  NAU Frutos do Mar · Orla da Ponte JK, SCE Sul · Brasília — DF
</footer>

<script>
  // Pacote tabs
  (function() {
    const tabs = document.querySelectorAll('.pacote-tab');
    const panels = document.querySelectorAll('.pacote-panel');
    tabs.forEach(tab => {
      tab.addEventListener('click', () => {
        const target = tab.dataset.pacote;
        tabs.forEach(t => t.classList.toggle('active', t.dataset.pacote === target));
        panels.forEach(p => p.classList.toggle('active', p.dataset.pacote === target));
        // Smooth scroll up to keep cardápio header in view
        const cardapio = document.getElementById('cardapio');
        if (cardapio) {
          const top = cardapio.getBoundingClientRect().top + window.scrollY - 80;
          if (window.scrollY > top + 100) {
            window.scrollTo({ top, behavior: 'smooth' });
          }
        }
      });
    });
  })();
</script>

<script>
  // Auto-print quando o PDF estiver pronto
  (function() {
    function ready() {
      // Aguarda fontes carregarem
      const fontsReady = document.fonts && document.fonts.ready
        ? document.fonts.ready
        : Promise.resolve();
      fontsReady.then(function() {
        // Aguarda imagens carregarem
        const imgs = Array.from(document.images);
        const imgsReady = Promise.all(imgs.map(function(img) {
          if (img.complete) return Promise.resolve();
          return new Promise(function(resolve) {
            img.addEventListener('load', resolve);
            img.addEventListener('error', resolve);
          });
        }));
        imgsReady.then(function() {
          // Pequena folga para o layout estabilizar
          setTimeout(function() {
            /* print disabled for web view */
          }, 600);
        });
      });
    }
    if (document.readyState === 'complete') {
      ready();
    } else {
      window.addEventListener('load', ready);
    }
  })();
</script>



</body></html>

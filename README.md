<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="theme-color" content="#f7f4ef">
  <title>Sobre eu</title>
  <style>
    :root {
      color-scheme: light;
      --ink: #282a35;
      --muted: #777986;
      --accent: #6d5ce8;
      --paper: #fff;
      --line: #eceaf2;
    }
    * { box-sizing: border-box; }
    body {
      margin: 0;
      min-height: 100vh;
      padding: 32px 20px;
      display: grid;
      place-items: center;
      background: #f7f4ef;
      color: var(--ink);
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    }
    .card {
      width: min(100%, 760px);
      overflow: hidden;
      border: 1px solid rgba(40, 42, 53, .06);
      border-radius: 28px;
      background: var(--paper);
      box-shadow: 0 24px 70px rgba(49, 42, 77, .10);
    }
    .top {
      padding: 54px clamp(26px, 7vw, 64px) 42px;
      background: linear-gradient(135deg, #f0edff 0%, #fff7ec 100%);
    }
    .eyebrow {
      margin: 0 0 18px;
      color: var(--accent);
      font-size: .76rem;
      font-weight: 800;
      letter-spacing: .14em;
      text-transform: uppercase;
    }
    h1 {
      max-width: 560px;
      margin: 0;
      font-size: clamp(2.4rem, 7vw, 4.2rem);
      line-height: 1.04;
      letter-spacing: -.055em;
    }
    h1 span { color: var(--accent); }
    .intro {
      max-width: 500px;
      margin: 20px 0 0;
      color: #656675;
      font-size: 1.05rem;
      line-height: 1.75;
    }
    .content { padding: 38px clamp(26px, 7vw, 64px) 48px; }
    h2 { margin: 0; font-size: 1.2rem; letter-spacing: -.02em; }
    .hint { margin: 8px 0 22px; color: var(--muted); font-size: .94rem; }
    .languages { display: grid; grid-template-columns: repeat(auto-fit, minmax(190px, 1fr)); gap: 12px; }
    .language {
      display: flex;
      align-items: center;
      gap: 14px;
      min-height: 76px;
      padding: 15px 17px;
      border: 1px solid var(--line);
      border-radius: 16px;
      background: #fff;
    }
    .flag { font-size: 1.75rem; line-height: 1; }
    .language strong { display: block; font-size: .98rem; }
    .language small { display: block; margin-top: 4px; color: var(--muted); font-size: .82rem; }
    footer {
      margin-top: 34px;
      padding-top: 20px;
      border-top: 1px solid var(--line);
      color: var(--muted);
      font-size: .85rem;
      text-align: center;
    }
    @media (max-width: 480px) {
      body { padding: 16px; }
      .card { border-radius: 22px; }
      .top { padding-top: 40px; }
    }
  </style>
</head>
<body>
  <main class="card">
    <section class="top" aria-labelledby="title">
      <p class="eyebrow">um pouco sobre eu</p>
      <h1>oi, eu sou <span>shiizetsu</span>.</h1>
      <p class="intro">acho que eu deveria aprender melhorar minhas habilidade em java script, mas fazer o que</p>
    </section>
    <section class="content" aria-labelledby="languages-title">
      <h2 id="languages-title">idiomas que eu conheço</h2>
      <p class="hint">depende, eu sei de outras.</p>
      <div class="languages">
        <div class="language"><span class="flag" aria-hidden="true">🇧🇷</span><div><strong>Português</strong><small>nativo (C2)</small></div></div>
        <div class="language"><span class="flag" aria-hidden="true">🇺🇸</span><div><strong>Inglês</strong><small>quase fluente (C1)</small></div></div>
        <div class="language"><span class="flag" aria-hidden="true">🇪🇸</span><div><strong>Espanhol</strong><small>Intermediário (B2)</small></div></div>
      </div>
      <footer>feito com o claude im ngl · <span id="year"></span></footer>
    </section>
  </main>
  <script>document.getElementById('year').textContent = new Date().getFullYear();</script>
</body>
</html>

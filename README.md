<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Central de Downloads · UP</title>
  <!-- Font Awesome para ícones modernos -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Roboto, system-ui, -apple-system, sans-serif;
      background: radial-gradient(circle at 20% 20%, #0f172a, #020617);
      color: #f1f5f9;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 24px 16px;
    }

    .container {
      max-width: 600px;
      width: 100%;
      margin: 0 auto;
    }

    /* ===== CARDS ===== */
    .card {
      background: rgba(255, 255, 255, 0.05);
      backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.08);
      border-radius: 36px;
      padding: 28px 24px;
      margin-bottom: 24px;
      box-shadow: 0 25px 40px -15px rgba(0, 0, 0, 0.7);
      transition: transform 0.2s ease, box-shadow 0.3s ease;
    }

    .card:hover {
      transform: translateY(-3px);
      box-shadow: 0 30px 50px -18px #000000cc;
    }

    /* ===== HERO ===== */
    .hero {
      text-align: center;
      padding: 18px 16px 28px;
      background: rgba(255, 255, 255, 0.02);
      border-bottom: 1px solid rgba(255, 255, 255, 0.03);
    }

    .logo {
      width: 84px;
      height: 84px;
      margin: 0 auto 16px;
      background: linear-gradient(145deg, #25D366, #128C7E);
      border-radius: 30px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 40px;
      color: #0b1a0e;
      box-shadow: 0 12px 20px -8px #128c7e55;
    }

    h1 {
      font-size: 2rem;
      font-weight: 700;
      letter-spacing: -0.3px;
      background: linear-gradient(to right, #e2e8f0, #b9c7e0);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      margin-bottom: 6px;
    }

    .subhead {
      font-size: 1rem;
      color: #94a3b8;
      margin-bottom: 22px;
      font-weight: 400;
      letter-spacing: 0.2px;
    }

    /* ===== BOTÕES ===== */
    .btn {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 12px;
      text-decoration: none;
      color: white;
      font-weight: 600;
      font-size: 1.05rem;
      padding: 15px 18px;
      border-radius: 60px;
      margin: 12px 0 8px;
      transition: all 0.2s ease;
      border: 1px solid rgba(255, 255, 255, 0.04);
      letter-spacing: 0.3px;
      background: rgba(255, 255, 255, 0.03);
      backdrop-filter: blur(4px);
    }

    .btn i {
      font-size: 1.3rem;
      width: 28px;
      text-align: center;
    }

    .btn:hover {
      transform: scale(1.01) translateY(-2px);
      filter: brightness(1.12);
      box-shadow: 0 16px 28px -8px rgba(0, 0, 0, 0.5);
    }

    .btn-whatsapp {
      background: #25D366;
      color: #052e16;
      border-color: #34eb7a;
    }

    .btn-whatsapp i {
      color: #052e16;
    }

    .btn-group {
      background: #075e54;
      border-color: #128C7E;
    }

    .btn-download {
      background: #2563eb;
      border-color: #3b82f6;
      color: white;
    }

    .btn-download i {
      color: #bfdbfe;
    }

    /* ===== CÓDIGO ===== */
    .code-box {
      background: rgba(0, 0, 0, 0.5);
      backdrop-filter: blur(4px);
      border-radius: 40px;
      padding: 12px 20px;
      margin: 16px 0 8px;
      display: inline-block;
      border: 1px solid #2563eb55;
      font-weight: 600;
      font-size: 1.1rem;
      color: #93c5fd;
      letter-spacing: 2px;
      box-shadow: 0 0 12px #2563eb22;
    }

    .code-box i {
      margin-right: 12px;
      color: #60a5fa;
    }

    .small-note {
      font-size: 0.82rem;
      color: #8896b0;
      margin-top: 12px;
      line-height: 1.5;
      border-top: 1px dashed #334155;
      padding-top: 14px;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .small-note i {
      color: #facc15;
      font-size: 1rem;
    }

    /* ===== RODAPÉ ===== */
    footer {
      text-align: center;
      color: #475569;
      font-size: 0.8rem;
      padding: 12px 0 0;
      letter-spacing: 0.4px;
      border-top: 1px solid #1e293b;
      margin-top: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      flex-wrap: wrap;
    }

    footer i {
      color: #2563eb;
    }

    /* ===== RESPONSIVO ===== */
    @media (max-width: 460px) {
      .card {
        padding: 20px 16px;
        border-radius: 28px;
      }
      .btn {
        font-size: 0.95rem;
        padding: 14px 16px;
      }
      h1 {
        font-size: 1.7rem;
      }
    }
  </style>
</head>
<body>
<div class="container">

  <!-- CARD PRINCIPAL / HERO -->
  <div class="card hero">
    <div class="logo">
      <i class="fas fa-cloud-download-alt"></i>
    </div>
    <h1>Central de Downloads</h1>
    <p class="subhead">
      <i class="fas fa-arrow-right" style="color: #38bdf8; margin-right: 8px;"></i>
      Acesse o material pelos botões abaixo
    </p>

    <!-- WhatsApp Pessoal -->
    <a class="btn btn-whatsapp" href="https://wa.me/5561992331249" target="_blank" rel="noopener noreferrer">
      <i class="fab fa-whatsapp"></i> Falar no WhatsApp
    </a>

    <!-- Grupo WhatsApp -->
    <a class="btn btn-group" href="https://chat.whatsapp.com/KCf5DwFhEKE4KqsaIMdUld?s=cl&p=a&mlu=4&ilr=4" target="_blank" rel="noopener noreferrer">
      <i class="fas fa-users"></i> Entrar no Grupo
    </a>
  </div>

  <!-- CARD ATIVADOR ANTI-BLOQUEIO -->
  <div class="card">
    <div style="display: flex; align-items: center; gap: 12px; margin-bottom: 12px;">
      <i class="fas fa-shield-alt" style="font-size: 2rem; color: #38bdf8;"></i>
      <h2 style="font-size: 1.4rem; font-weight: 600; letter-spacing: -0.2px;">Ativador Anti-Bloqueio</h2>
    </div>

    <p style="color: #cbd5e1; margin-bottom: 18px; line-height: 1.6;">
      <i class="fas fa-microchip" style="color: #60a5fa; margin-right: 8px;"></i>
      Diagnóstico e configuração de conexão para Android.
    </p>

    <!-- Botão Download -->
    <a class="btn btn-download" href="https://aftv.news/5812236" target="_blank" rel="noopener noreferrer">
      <i class="fas fa-download"></i> Acessar Download
    </a>

    <!-- Código com ícone -->
    <div style="display: flex; justify-content: center;">
      <div class="code-box">
        <i class="fas fa-key"></i> Código: 5812236
      </div>
    </div>

    <!-- Dica extra -->
    <div class="small-note">
      <i class="fas fa-exclamation-triangle"></i>
      <span>Se aparecer erro de conexão, verifique primeiro sua internet e configurações do dispositivo.</span>
    </div>
  </div>

  <!-- RODAPÉ -->
  <footer>
    <i class="fas fa-database"></i>
    <span>© 2026 · Central de Downloads</span>
    <i class="fas fa-circle" style="font-size: 0.3rem; color: #475569;"></i>
    <span style="display: inline-flex; gap: 4px; align-items: center;">
      <i class="fas fa-arrow-up" style="color: #22d3ee;"></i> up
    </span>
  </footer>

</div>
</body>
</html>

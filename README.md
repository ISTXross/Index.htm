<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Aprenda Programação | Ross</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #0d1117;
  color: #fff;
}

.screen {
  display: none;
  padding: 40px 20px;
  max-width: 800px;
  margin: auto;
}

.active {
  display: block;
}

h1, h2 {
  text-align: center;
}

.button {
  display: block;
  margin: 20px auto;
  padding: 15px;
  width: 80%;
  max-width: 300px;
  text-align: center;
  background: #2563eb;
  border-radius: 10px;
  cursor: pointer;
}

.button:hover {
  background: #1d4ed8;
}

.card {
  background: #161b22;
  padding: 20px;
  border-radius: 10px;
  margin-top: 20px;
}

</style>
</head>

<body>

<!-- TELA INICIAL -->
<div id="home" class="screen active">
  <h1>Aprender Programação 🚀</h1>
  <p style="text-align:center;">Escolha o que você quer aprender</p>

  <div class="button" onclick="go('ebook')">📘 Começar E-book</div>
</div>

<!-- E-BOOK -->
<div id="ebook" class="screen">
  <h1>E-book: Aprender Programação do Zero</h1>

  <div class="card">
    <h2>📌 Introdução</h2>
    <p>Programação é a habilidade de criar soluções usando código. Você não precisa ser um gênio — precisa de prática.</p>
  </div>

  <div class="card">
    <h2>💻 HTML</h2>
    <p>É a estrutura dos sites. Tudo começa aqui.</p>
  </div>

  <div class="card">
    <h2>🎨 CSS</h2>
    <p>Responsável pelo design e aparência do site.</p>
  </div>

  <div class="card">
    <h2>⚡ JavaScript</h2>
    <p>Faz o site ter interatividade.</p>
  </div>

  <div class="card">
    <h2>🚀 Como evoluir</h2>
    <p>Pratique todos os dias, crie projetos e publique no GitHub.</p>
  </div>

  <div class="button" onclick="go('final')">Continuar</div>
</div>

<!-- FINAL (VENDA) -->
<div id="final" class="screen">
  <h1>🔥 Quer aprender de verdade?</h1>

  <div class="card">
    <p>
      Se você quer evoluir rápido e ter acompanhamento, eu posso te ajudar diretamente.
    </p>
  </div>

  <div class="button" onclick="whatsapp()">
    Falar comigo no WhatsApp
  </div>
</div>

<script>
function go(screen) {
  document.querySelectorAll(".screen").forEach(s => s.classList.remove("active"));
  document.getElementById(screen).classList.add("active");
}

function whatsapp() {
  window.open("https://wa.me/5514997617846", "_blank");
}
</script>

</body>
</html>

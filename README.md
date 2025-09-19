<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Casa do Focus</title>
<style>
body {margin:0; padding:0; font-family: Arial, sans-serif; background-color: #000; color: #0f0; position: relative; min-height: 100vh; overflow-x: hidden;}
.emoji-bg {position: absolute; font-size: 20px; opacity: 0.08; animation: float 15s linear infinite;}
@keyframes float {0% {transform: translateY(0) rotate(0deg);} 50% {transform: translateY(-50px) rotate(180deg);} 100% {transform: translateY(0) rotate(360deg);}}
header {text-align:center; padding:40px 20px 10px;}
header h1 {font-size:3em; margin:0; color:#0f0;}
header p {font-size:1.2em; color:#0a0; margin-top:10px;}
.course-buttons {display:flex; justify-content:center; gap:30px; flex-wrap:wrap; margin:30px 0;}
button {background-color:#0f0; color:#000; font-weight:bold; border:none; padding:15px 30px; cursor:pointer; font-size:1.2em; border-radius:12px; transition: all 0.3s ease;}
button:hover {transform: scale(1.08); box-shadow:0 0 10px #0f0,0 0 20px #0f0;}
.small-button {padding:12px 25px; font-size:1em;}
.benefits-section {max-width:900px; margin:50px auto; padding:0 20px; text-align:center;}
.benefits-section h2 {color:#0f0; font-size:2em; margin-bottom:30px;}
.benefits {display:flex; flex-wrap:wrap; justify-content:center; gap:25px;}
.benefit {background-color: rgba(0,255,0,0.05); border:2px solid #0f0; border-radius:15px; padding:20px; width:250px; transition: all 0.3s ease; cursor:default;}
.benefit:hover {transform: scale(1.05); box-shadow:0 0 15px #0f0,0 0 30px #0f0;}
.benefit-icon {font-size:2.5em; margin-bottom:15px;}
.benefit h3 {font-size:1.2em; margin-bottom:10px; color:#0f0;}
.benefit p {font-size:0.95em; color:#0a0;}
.reviews-section {max-width:900px; margin:50px auto; padding:0 20px;}
.reviews-section h2 {text-align:center; font-size:2em; color:#0f0; margin-bottom:20px;}
.reviews {display:grid; grid-template-columns:repeat(auto-fit,minmax(250px,1fr)); gap:20px;}
.review {background-color: rgba(0,255,0,0.05); border:2px solid #0f0; padding:15px; border-radius:15px; transition: all 0.3s ease; cursor:pointer;}
.review.male{border-color:#00f;} 
.review.female{border-color:#ff69b4;}
.review.expanded{transform: scale(1.05); background-color:rgba(0,255,0,0.15); padding:25px; box-shadow:0 0 15px #0f0,0 0 30px #0f0; z-index:1;}
.review .name {font-weight:bold; color:#0f0;}
.review .time, .review .course {font-size:0.9em; color:#0a0;}
.review .message {margin-top:5px;}
.support-btn {position:fixed; bottom:20px; right:20px; 
background: linear-gradient(45deg,#00ff00,#0a0); color:#000; padding:18px 28px; font-size:1.3em; font-weight:bold; border:2px solid #0f0; border-radius:50px; cursor:pointer; transition: all 0.3s ease; box-shadow:0 0 15px #0f0,0 0 30px #0a0; z-index:1000;}
.support-btn:hover {transform: scale(1.1);}
#chat-popup {position:fixed; bottom:80px; right:20px; width:260px; height:360px; background:rgba(0,0,0,0.9); border:1px solid #444; border-radius:15px; display:none; flex-direction:column; overflow-y:auto; padding:10px; z-index:1000; box-shadow:0 0 15px rgba(255,255,255,0.1); opacity:0; transform:translateY(50px); transition:all 0.5s ease;}
#chat-popup.show {opacity:1; transform:translateY(0);}
.bot,.user {padding:8px 12px;border-radius:10px;margin:5px 0;max-width:80%;position:relative;}
.bot{background:#075E54;color:white;align-self:flex-start;}
.user{background:#25D366;color:black;align-self:flex-end;}
.time{font-size:10px;color:rgba(255,255,255,0.7);position:absolute;bottom:-12px;right:8px;}
.menu{margin-top:auto;display:flex;flex-direction:column;gap:10px;}
.menu button{background:#202c33;color:white;border:none;padding:10px;border-radius:8px;cursor:pointer;transition:0.2s;font-size:0.9em;}
.menu button:active{transform:scale(1.05); box-shadow:0 0 10px #0f0,0 0 20px #0f0;}
.typing{display:flex;gap:4px;align-items:center;margin:5px 0;}
.dot{width:6px;height:6px;background:white;border-radius:50%;animation:blink 1s infinite;}
.dot:nth-child(2){animation-delay:0.2s;}
.dot:nth-child(3){animation-delay:0.4s;}
@keyframes blink{0%,80%,100%{opacity:0;}40%{opacity:1;}}
@media (max-width:768px){header h1{font-size:2.5em;}.benefits {flex-direction:column; align-items:center;}.course-buttons {flex-direction:column; gap:15px;}}
</style>
</head>
<body>

<script>
for(let i=0;i<50;i++){
  let e=document.createElement('div');
  e.className='emoji-bg';
  e.style.left=Math.random()*100+'vw';
  e.style.top=Math.random()*100+'vh';
  e.style.fontSize=Math.random()*30+15+'px';
  e.innerText='⚠';
  document.body.appendChild(e);
}
</script>

<header>
<h1>Casa do Focus</h1>
<p>Aprenda estratégias de Marketing Digital e gere renda extra de forma prática!</p>
</header>

<div class="course-buttons">
  <button id="btn1" onclick="window.open('https://global.tribopay.com.br/0bazx?affh=vx5v9zrvcv','_blank')">Método de Renda Extra</button>
  <button id="btn2" class="small-button" onclick="window.open('https://global.tribopay.com.br/oo5edcxmhq?affh=qs90rgb8zf','_blank')">Renda Extra Na Internet - Do Zero à Primeira Venda em 15 Dias</button>
</div>

<section class="benefits-section">
<h2>O que você vai ganhar</h2>
<div class="benefits">
<div class="benefit"><div class="benefit-icon">💻</div><h3>Acesso completo</h3><p>Aprenda passo a passo todas as estratégias de marketing digital.</p></div>
<div class="benefit"><div class="benefit-icon">🚀</div><h3>Resultados rápidos</h3><p>Descubra técnicas que geram resultados reais em pouco tempo.</p></div>
<div class="benefit"><div class="benefit-icon">💰</div><h3>Renda extra garantida</h3><p>Transforme conhecimento em dinheiro de forma prática.</p></div>
<div class="benefit"><div class="benefit-icon">🎯</div><h3>Estratégias testadas</h3><p>Use métodos aplicados com sucesso por outros alunos.</p></div>
</div>
</section>

<section class="reviews-section">
<h2>Depoimentos de Quem Já Fez</h2>
<div class="reviews">
<div class="review female"><div class="name">Ana Silva</div><div class="time">19:30</div><div class="course">Método de Renda Extra</div><div class="message">Eu amei o curso! Muito fácil de entender e aplicar.</div></div>
<div class="review male"><div class="name">Carlos Souza</div><div class="time">14:15</div><div class="course">Renda Extra Na Internet - Do Zero à Primeira Venda em 15 Dias</div><div class="message">Excelente conteúdo! Recomendo para todos que querem aprender marketing digital.</div></div>
<div class="review female"><div class="name">Juliana Mendes</div><div class="time">10:05</div><div class="course">Método de Renda Extra</div><div class="message">O curso mudou minha forma de pensar no marketing, vale muito a pena!</div></div>
<div class="review male"><div class="name">Bruno Lima</div><div class="time">12:20</div><div class="course">Método de Renda Extra</div><div class="message">Aprendi muitas estratégias de marketing que já estou aplicando.</div></div>
<div class="review female"><div class="name">Mariana Costa</div><div class="time">16:45</div><div class="course">Renda Extra Na Internet - Do Zero à Primeira Venda em 15 Dias</div><div class="message">O conteúdo é claro e direto ao ponto, adorei!</div></div>
</div>
</section>

<button class="support-btn" onclick="abrirSuporte()">Suporte 🟢</button>

<div id="chat-popup">
<div class="bot">Olá 👋 Escolha uma opção abaixo:<div class="time" id="time0"></div></div>
<div class="menu">
<button onclick="responder('Como começar no marketing digital?')">Como começar no marketing digital?</button>
<button onclick="responder('Quais ferramentas usar para vender online?')">Ferramentas para vender online</button>
<button onclick="responder('Como gerar renda extra rapidamente?')">Como gerar renda extra</button>
<button onclick="responder('Dicas para anúncios no Instagram e Facebook')">Dicas de anúncios</button>
<button onclick="responder('Suporte sobre cursos adquiridos')">Suporte sobre cursos</button>
</div>
</div>

<script>
// Depoimentos expansíveis
document.querySelectorAll('.review').forEach(r=>{r.addEventListener('click',()=>{r.classList.toggle('expanded');});});

// Hora
function horaAtual(){let agora=new Date();return agora.toLocaleTimeString([], {hour:'2-digit', minute:'2-digit'});}
document.getElementById("time0").textContent=horaAtual();

// Suporte
function abrirSuporte(){
  const chat=document.getElementById('chat-popup');
  if(!chat.classList.contains('show')){
    chat.style.display='flex';
    setTimeout(()=>chat.classList.add('show'),50);
  }else{
    chat.classList.remove('show');
    setTimeout(()=>chat.style.display='none',500);
  }
}

// Respostas cativantes
function responder(opcao){
  let chat=document.getElementById("chat-popup");
  let userMsg=document.createElement("div"); userMsg.className="user";
  userMsg.innerHTML=opcao+`<div class="time">${horaAtual()}</div>`;
  chat.insertBefore(userMsg, chat.querySelector(".menu"));
  let typing=document.createElement("div"); typing.className="typing bot";
  typing.innerHTML='<div class="dot"></div><div class="dot"></div><div class="dot"></div>';
  chat.insertBefore(typing, chat.querySelector(".menu"));
  chat.scrollTop=chat.scrollHeight;
  setTimeout(()=>{
    typing.remove();
    let botMsg=document.createElement("div"); botMsg.className="bot";
    botMsg.innerHTML="Essa é uma dica incrível! 😉✨ <br> Clique em um dos cursos acima e comece agora!<div class='time'>"+horaAtual()+"</div>";
    chat.insertBefore(botMsg, chat.querySelector(".menu"));
    chat.scrollTop=chat.scrollHeight;
  },1000);
}
</script>

</body>
</html>

# Regalo-para-sumi

<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#ffe5ef">
<title>Un universo para Sumi ♡</title>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html { scroll-behavior: smooth; }

body {
  font-family: Georgia, serif;
  background: linear-gradient(145deg,#fff1f6,#fbdce9,#ffeaf2);
  color: #89516b;
  text-align: center;
  overflow-x: hidden;
}

section {
  padding: 70px 20px;
  position: relative;
  z-index: 1;
}

h1 {
  color: #d76e9b;
  font-size: clamp(40px,10vw,65px);
  margin: 20px 0;
}

h2 {
  color: #cf7298;
  font-size: 27px;
  margin-bottom: 25px;
}

p {
  line-height: 1.9;
  font-size: 17px;
}

button {
  border: none;
  background: #e78caf;
  color: white;
  padding: 14px 25px;
  border-radius: 30px;
  font-size: 16px;
  cursor: pointer;
  margin: 10px;
  transition: .3s;
}

button:active {
  transform: scale(.95);
}

.hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.subtitle {
  max-width: 380px;
  margin: 10px auto 25px;
}

.card {
  background: rgba(255,255,255,.75);
  max-width: 550px;
  margin: 20px auto;
  padding: 30px 23px;
  border-radius: 25px;
  box-shadow: 0 8px 30px #d88eaa25;
}

.letter {
  text-align: left;
  line-height: 2;
  white-space: pre-line;
}

.heart {
  position: fixed;
  bottom: -40px;
  color: #e58caf;
  pointer-events: none;
  z-index: 0;
  animation: float 7s linear forwards;
}

@keyframes float {
  to {
    transform: translateY(-110vh) rotate(360deg);
    opacity: 0;
  }
}

#game {
  display: grid;
  grid-template-columns: repeat(3,1fr);
  gap: 12px;
  max-width: 340px;
  margin: 25px auto;
}

.heart-box {
  height: 80px;
  border-radius: 17px;
  border: 2px solid #f0b6cc;
  background: #ffe3ed;
  color: #d76e9b;
  font-size: 27px;
  margin: 0;
}

.heart-box:disabled {
  opacity: 1;
}

.found {
  background: #f8bfd4;
}

#surprise {
  display: none;
  animation: appear 1.2s ease;
  margin-top: 30px;
}

@keyframes appear {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

input[type=file] {
  max-width: 100%;
  margin: 20px 0;
}

audio {
  width: 100%;
  margin-top: 15px;
}

footer {
  padding: 35px 15px;
  color: #bb7795;
}

@media(max-width:400px) {
  section { padding: 55px 14px; }
  .card { padding: 25px 17px; }
  h2 { font-size: 24px; }
}
</style>
</head>

<body>

<section class="hero">

<p>♡ Un pequeño detalle para alguien especial ♡</p>

<h1>Para Sumi</h1>

<p class="subtitle">
Hay personas que hacen que el mundo
sea un poquito más bonito...
y tú eres una de ellas.
</p>

<button onclick="document.getElementById('inicio').scrollIntoView()">
Abrir mi sorpresa ♡
</button>

<p style="margin-top:35px">♡ ♡ ♡</p>

</section>

<section id="inicio">

<h2>Quiero decirte algo...</h2>

<div class="card">

<p>
No necesitas una ocasión especial
para recibir un detalle bonito.

Hoy simplemente quería regalarte
un pequeño espacio lleno de cariño.
</p>

<h2 style="margin-top:25px">
Te quiero mucho ♡
</h2>

<p>
Eres la persona especial en mi vida.
</p>

</div>
</section>

<section>

<h2>Una carta para ti 💌</h2>

<div class="card letter">

Querida Sumi:

Quería dedicarte algo diferente,
algo que pudieras abrir y recordar
que hay alguien que te aprecia muchísimo.

A veces las palabras no son suficientes
para expresar lo importante que puede
llegar a ser una persona.

Quiero que sepas que te quiero mucho,
que eres una persona especial en mi vida
y que me alegra poder compartir
momentos contigo.

Gracias por ser tú.

Con mucho cariño,
alguien que te quiere ♡

</div>
</section>

<section>

<h2>Una canción para ti 🎵</h2>

<div class="card">

<p>
Esta canción será parte de tu pequeña sorpresa.
</p>

<input type="file" id="musicFile" accept="audio/*">

<audio id="audio" controls>
Tu navegador no admite audio.
</audio>

<p style="font-size:13px;margin-top:15px">
Selecciona una canción de tu dispositivo.
</p>

</div>
</section>

<section>

<h2>Un pequeño juego ❤️</h2>

<div class="card">

<p>
He escondido 5 corazones entre estas casillas.
¿Puedes encontrarlos todos?
</p>

<p id="counter" style="margin-top:15px">
Corazones encontrados: 0 / 5
</p>

<div id="game"></div>

<div id="surprise">

<h2>¡Los encontraste todos! 💗</h2>

<p>
Has descubierto todos los corazones,
pero todavía queda algo por decirte...
</p>

<h1>♡ Sumi ♡</h1>

<p>
Te quiero mucho.
Eres una persona muy especial
en mi vida.
</p>

</div>
</div>
</section>

<section>

<h2>Hasta el infinito ♡</h2>

<div class="card">

<p>
Si pudiera guardar este pequeño momento
en algún lugar, lo guardaría aquí.
</p>

<h1>Para Sumi</h1>

<p>
Con muchísimo cariño. 💗
</p>

</div>
</section>

<footer>
Hecho con cariño ♡
<br>
Un pequeño universo para Sumi.
</footer>

<script>

function createHeart() {

const heart = document.createElement("div");

heart.className = "heart";
heart.textContent = "♡";

heart.style.left = Math.random()*100+"vw";
heart.style.fontSize = (15+Math.random()*25)+"px";
heart.style.animationDuration = (5+Math.random()*5)+"s";

document.body.appendChild(heart);

setTimeout(() => heart.remove(),10000);

}

setInterval(createHeart,650);


// REPRODUCTOR DE MÚSICA

const musicFile = document.getElementById("musicFile");
const audio = document.getElementById("audio");

let currentURL = null;

musicFile.addEventListener("change",function() {

const file = this.files[0];

if(file) {

if(currentURL) URL.revokeObjectURL(currentURL);

currentURL = URL.createObjectURL(file);

audio.src = currentURL;
audio.load();

}

});


// JUEGO

const game = document.getElementById("game");

let found = 0;

const hiddenHearts = new Set();

while(hiddenHearts.size < 5) {
hiddenHearts.add(Math.floor(Math.random()*9));
}

for(let i=0;i<9;i++) {

const cell = document.createElement("button");

cell.className = "heart-box";
cell.textContent = "?";
cell.setAttribute("aria-label","Casilla misteriosa");

cell.addEventListener("click",function() {

if(cell.disabled) return;

cell.disabled = true;

if(hiddenHearts.has(i)) {

cell.textContent = "❤️";
cell.classList.add("found");

found++;

document.getElementById("counter").textContent =
"Corazones encontrados: "+found+" / 5";

if(found===5) {

document.getElementById("surprise").style.display="block";

document.getElementById("surprise").scrollIntoView({
behavior:"smooth",
block:"center"
});

}

} else {

cell.textContent = "♡";
cell.style.opacity = ".5";

}

});

game.appendChild(cell);

}

</script>

</body>
</html>

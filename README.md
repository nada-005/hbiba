
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Lik NADA ❤️</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --pink: #ff4f87;
  --light-pink: #ffb6cc;
  --black: #090609;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: Georgia, serif;
  background: #fff3f7;
  color: #542a3b;
  overflow-x: hidden;
}

button {
  font-family: inherit;
  cursor: pointer;
}

/* OPENING SCREEN */

#intro {
  position: fixed;
  inset: 0;
  z-index: 9999;
  background:
    radial-gradient(circle, #32101f 0%, #13080f 48%, #050305 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 20px;
  overflow: hidden;
  transition: opacity 1s, visibility 1s;
}

#intro.hide {
  opacity: 0;
  visibility: hidden;
  pointer-events: none;
}

.intro-content {
  position: relative;
  z-index: 2;
  width: 100%;
}

.small-title {
  color: #ffb3cc;
  font-family: Arial, sans-serif;
  font-size: 12px;
  letter-spacing: 4px;
  margin-bottom: 30px;
  animation: fadeIn 1s both;
}

.name {
  color: var(--pink);
  font-family: "Segoe Print", "Comic Sans MS", cursive;
  font-size: clamp(65px, 14vw, 130px);
  font-weight: bold;
  line-height: 1.2;
  text-shadow: 0 0 25px #ff286b55;
  overflow: hidden;
  white-space: nowrap;
  width: 0;
  margin: auto;
  border-right: 3px solid var(--light-pink);
  animation:
    writeName 1.5s steps(4, end) .5s forwards,
    blink .7s step-end infinite;
}

.love-text {
  margin-top: 18px;
  color: #ff729e;
  font-family: "Segoe Print", "Comic Sans MS", cursive;
  font-size: clamp(20px, 5vw, 39px);
  font-weight: bold;
  opacity: 0;
  animation: showLove 1s 2s forwards;
  text-shadow: 0 0 20px #ff3b7850;
}

.intro-sub {
  color: #e8b5c6;
  font: 13px Arial, sans-serif;
  margin-top: 20px;
  opacity: 0;
  animation: fadeIn 1s 2.6s forwards;
}

.enter-btn {
  border: 1px solid #ff80a8;
  color: white;
  background: linear-gradient(135deg, #ff6595, #a51b4c);
  border-radius: 50px;
  padding: 15px 25px;
  margin-top: 30px;
  font-size: 14px;
  box-shadow: 0 0 30px #ff347844;
  opacity: 0;
  animation: fadeIn 1s 3s forwards;
  transition: .3s;
}

.enter-btn:hover {
  transform: scale(1.06);
  box-shadow: 0 0 40px #ff347899;
}

@keyframes writeName {
  to { width: 4ch; }
}

@keyframes blink {
  50% { border-color: transparent; }
}

@keyframes showLove {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(12px); }
  to { opacity: 1; transform: translateY(0); }
}

/* FALLING ROSES */

.petal {
  position: absolute;
  top: -60px;
  color: #ff315f;
  font-size: 24px;
  pointer-events: none;
  animation: fall linear forwards;
  filter: drop-shadow(0 0 6px #ff174455);
}

@keyframes fall {
  from {
    transform: translateY(-5vh) rotate(0);
    opacity: 1;
  }
  to {
    transform: translateY(115vh) rotate(600deg);
    opacity: 0;
  }
}

/* MAIN WEBSITE */

nav {
  padding: 23px 8%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  color: #d74779;
  font-weight: bold;
  font-size: 20px;
}

.nav-label {
  font-size: 12px;
  color: #9e7486;
}

.hero {
  min-height: 82vh;
  padding: 40px 8%;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 50px;
  flex-wrap: wrap;
}

.hero-text {
  flex: 1 1 300px;
  max-width: 520px;
}

.tag {
  display: inline-block;
  background: white;
  color: #d74779;
  border: 1px solid #f7c4d5;
  border-radius: 50px;
  padding: 10px 16px;
  font: 12px Arial, sans-serif;
}

.hero h1 {
  font-size: clamp(55px, 8vw, 90px);
  margin: 25px 0;
  color: #4e2a3b;
}

.hero h1 span {
  color: #df5787;
  font-style: italic;
}

.hero p {
  color: #936b7d;
  font: 16px/1.9 Arial, sans-serif;
}

.btn {
  border: none;
  background: linear-gradient(135deg, #f48daf, #d74779);
  color: white;
  border-radius: 40px;
  padding: 15px 22px;
  margin-top: 25px;
  box-shadow: 0 8px 25px #d7477928;
  transition: .3s;
}

.btn:hover {
  transform: translateY(-3px);
}

.rose-art {
  flex: 1 1 260px;
  max-width: 350px;
  min-height: 300px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  background: radial-gradient(circle, #ffe0eb, #fff5f8 65%, transparent 66%);
}

.rose-art span {
  font-size: clamp(130px, 25vw, 210px);
  filter: drop-shadow(0 15px 20px #d7477930);
  animation: float 4s ease-in-out infinite;
}

@keyframes float {
  50% { transform: translateY(-12px) rotate(4deg); }
}

.section {
  padding: 75px 20px;
  text-align: center;
}

.section h2 {
  font-size: clamp(30px, 5vw, 45px);
  margin: 15px 0;
}

.section > p {
  font: 15px/1.9 Arial, sans-serif;
  color: #936b7d;
}

.card {
  max-width: 680px;
  margin: 30px auto;
  padding: 35px;
  background: white;
  border: 1px solid #f5c6d7;
  border-radius: 25px;
  box-shadow: 0 15px 50px #d7477910;
  text-align: left;
}

.card p {
  font: 15px/2 Arial, sans-serif;
  color: #795364;
  margin-bottom: 15px;
}

.signature {
  color: #d74779 !important;
  font-weight: bold !important;
}

.gift {
  max-width: 650px;
  margin: 30px auto;
  padding: 35px 20px;
  border-radius: 25px;
  background: linear-gradient(135deg, white, #ffe4ed);
  border: 1px solid #f5c6d7;
}

.gift-icon {
  font-size: 60px;
}

#surprise-message {
  display: none;
  color: #795364;
  font: 16px/2 Arial, sans-serif;
  margin-top: 25px;
}

#surprise-message.show {
  display: block;
  animation: fadeIn .8s both;
}

footer {
  text-align: center;
  padding: 30px 15px;
  color: #a67e90;
  font: 13px Arial, sans-serif;
}

/* LETTER POPUP */

#letter-modal {
  position: fixed;
  inset: 0;
  background: #1b0a13aa;
  backdrop-filter: blur(7px);
  z-index: 500;
  display: none;
  align-items: center;
  justify-content: center;
  padding: 20px;
}

#letter-modal.show {
  display: flex;
}

.modal-card {
  position: relative;
  background: #fffafd;
  padding: 35px 25px;
  border-radius: 25px;
  max-width: 480px;
  width: 100%;
  text-align: center;
  animation: fadeIn .4s both;
}

.modal-card h2 {
  color: #d74779;
  margin: 15px 0;
}

.modal-card p {
  color: #795364;
  font: 15px/1.9 Arial, sans-serif;
}

.close-btn {
  position: absolute;
  right: 14px;
  top: 12px;
  border: none;
  background: #ffe2ec;
  color: #d74779;
  border-radius: 50%;
  width: 35px;
  height: 35px;
  font-size: 22px;
}

@media (max-width: 600px) {
  nav { padding: 20px; }
  .hero { text-align: center; padding: 35px 23px; gap: 20px; }
  .hero-text { flex-basis: 100%; }
  .rose-art { min-height: 230px; }
  .card { padding: 25px 20px; }
  .name { font-size: 70px; }
}
</style>
</head>

<body>

<!-- OPENING SCREEN -->
<div id="intro">
  <div class="intro-content">
    <div class="small-title">A SPECIAL MESSAGE FOR YOU ♡</div>

    <div class="name">NADA</div>

    <div class="love-text">KANBGHIIIIIIIIIK ❤️</div>

</script>

</body>
</html>

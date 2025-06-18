<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Madame Baby 🌸</title>
  <style>
    :root {
      --soft-pink: #ffe3ec;
      --pink-accent: #ff99c8;
      --button-hover: #ff69b4;
      --text-color: #3f3f3f;
    }

    body {
      margin: 0;
      font-family: 'Helvetica Neue', sans-serif;
      background-color: var(--soft-pink);
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }

    .card {
      background-color: white;
      padding: 2rem 2rem;
      border-radius: 1.5rem;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
      text-align: center;
      max-width: 380px;
      width: 90%;
    }

    h2 {
      color: var(--text-color);
      font-weight: 500;
      margin-bottom: 1.8rem;
    }

    button {
      background-color: var(--pink-accent);
      color: white;
      border: none;
      padding: 0.7rem 1.4rem;
      font-size: 1rem;
      border-radius: 999px;
      margin: 0.4rem;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: var(--button-hover);
    }

    img {
      max-width: 100%;
      border-radius: 1rem;
      margin-top: 1rem;
    }
  </style>
</head>
<body>
  <div class="card" id="card">
    <h2>Hello, madame baby.🌼</h2>
    <button onclick="nextQuestion()">→</button>
  </div>

  <script>
    const card = document.getElementById('card');

    function nextQuestion() {
      card.innerHTML = `
        <h2>Nananakit ba ang iyong kasukasuan?</h2>
        <button onclick="goodAnswer()"> Oo huhuhu</button>
        <button onclick="sunshineStart()"> Hindi naman</button>
      `;
    }

    function goodAnswer() {
      card.innerHTML = `
        <h2>What if i-exercise na yan</h2>
        <button onclick="inviteDate1()">Suree</button>
        <button onclick="finalNo()">Wag na, keri na'to</button>
      `;
    }
function inviteDate1() {
      card.innerHTML = `
        <h2>Are u free this coming Sunday in the afternoon? </h2>
        <button onclick="inviteDate()">Yaazz</button>
        <button onclick="finalNo()">Nopee</button>
      `;
    }

    function inviteDate() {
      card.innerHTML = `
        <h2>Then do you want to go on a jogging date with me?</h2>
        <button onclick="dateDetails()">Hmmm</button>
        <button onclick="finalNo()">ihh</button>
      `;
    }

    function dateDetails() {
      card.innerHTML = `
        <h2>Pretty pleasee</h2>
        <button onclick="confirmYes()">Shigi ne nge</button>
        <button onclick="confirmNo()">Ayaw q nga</button>
      `;
    }

    function confirmYes() {
      card.innerHTML = `
         <h2>Send a photo of pond naravit to confirm.</h2>
        
      `;
    }

    function confirmNo() {
      card.innerHTML = `
        <h2>AAAAAaaa sigi:33</h2>
      `;
    }

    function finalNo() {
      card.innerHTML = `
        <h2>AAAAAaaa sigi:33</h2>
      `;
    }

    // SUNSHINE PATH
    function sunshineStart() {
      card.innerHTML = `
        <h2>Tag-ulan na, hindi ka ba nilalamig?</h2>
        <button onclick="sunshineConfirm()">→</button>
      
      `;
    }

    function sunshineConfirm() {
      card.innerHTML = `
        <h2> What if i-coffee date na yan? uwuu</h2>
        <button onclick="sunshineYes()">shige</button>
        <button onclick="confirmNo()"> wag na, nak</button>
      `;
    }

    function sunshineYes() {
      card.innerHTML = `
        <h2>Yeheyy. Are u free ba this coming sunday?</h2>
          <button onclick="nextQuestion2()">→</button>
       `;
    }
    function nextQuestion2() {
      card.innerHTML = `
        <h2>If yes, seal the deal with pond naavit photoo.</h2>
      
      `;
    }
  </script>
</body>
</html>

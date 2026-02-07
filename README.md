<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Random Sustainability Word</title>

  <!-- Onest Font -->
  <link href="https://fonts.googleapis.com/css2?family=Onest:wght@300;400;600&display=swap" rel="stylesheet">

  <style>
    body {
      font-family: 'Onest', sans-serif;
      height: 100vh;
      margin: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(160deg, #012158, #000000);
      color: #e6f2ff;
    }

    .card {
      background: rgba(255, 255, 255, 0.12);
      border: 1px solid silver;
      border-radius: 16px;
      padding: 40px;
      text-align: center;
      box-shadow: 0 0 20px rgba(0,0,0,0.2);
      max-width: 400px;
      width: 90%;
    }

    h1 {
      margin-bottom: 20px;
      color: #e6f2ff;
      letter-spacing: 1px;
    }

    .word {
      font-size: 28px;
      font-weight: 600;
      color: #7ec8ff;
      margin: 20px 0;
      min-height: 40px;
    }

    button {
      background: #1e90ff;
      color: white;
      border: none;
      padding: 12px 24px;
      border-radius: 10px;
      font-size: 16px;
      cursor: pointer;
      transition: all 0.2s ease;
      font-family: 'Onest', sans-serif;
    }

    button:hover {
      background: silver;
      color: #0b2b44;
    }
  </style>
</head>

<body>

  <div class="card">
    <h1>Green Gestures</h1>
    <div class="word" id="wordDisplay">Click the button</div>
    <button onclick="pickWord()">Pick a Word</button>
  </div>

  <script>
    const words = [
      "Reduce",
      "Reuse",
      "Recycle",
      "Conserve",
      "Restore",
      "Electrify",
      "Harvest",
      "Balance",
      "Turn off lights",
      "Save water",
      "Use a bike",
      "Plant a tree",
      "Pick up trash",
      "Use reusable bag",
      "Segregate waste",
      "Refill bottle",
      "Avoid plastic"
    ];

    function pickWord() {
      const randomIndex = Math.floor(Math.random() * words.length);
      document.getElementById("wordDisplay").innerText = words[randomIndex];
    }
  </script>

    <p>Click to go back to <a href="https://blueprint-homepage.carrd.co/">homepage.</a></p>

</body>
</html>

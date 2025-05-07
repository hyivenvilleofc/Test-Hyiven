<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>The Hyven Trials</title>
  <style>
    body {
      margin: 0;
      font-family: 'Georgia', serif;
    }
    .slide {
      display: none;
      height: 100vh;
      width: 100vw;
      background-size: cover;
      background-position: center;
      position: relative;
    }
    .active {
      display: block;
    }
    .centered {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
    }
    .btn {
      background-color: red;
      color: white;
      border: none;
      padding: 15px 30px;
      font-size: 24px;
      cursor: pointer;
      border-radius: 10px;
      margin: 10px;
    }
    .title {
      font-size: 28px;
      font-weight: bold;
      color: white;
      text-shadow: 2px 2px 5px black;
      margin-bottom: 20px;
    }
    .next-text {
      color: white;
      position: absolute;
      bottom: 30px;
      right: 30px;
      font-size: 22px;
      text-shadow: 2px 2px 5px black;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <!-- Slide 1 -->
  <div id="slide1" class="slide active" style="background-image: url('https://i.imgur.com/ONkMu5q.png');">
    <div class="centered">
      <div class="title">THE HYVEN TRIALS:<br>FIND YOUR TRUE FORM</div>
      <button class="btn" onclick="nextSlide()">Start</button>
    </div>
  </div>

  <!-- Slide 2 -->
  <div id="slide2" class="slide" style="background-image: url('https://i.imgur.com/2EDLzS1.png');">
    <div class="centered">
      <div class="title">Muse kamu dari grup mana?</div>
      <button class="btn" onclick="chooseGroup('witch')">IVE</button>
      <button class="btn" onclick="chooseGroup('dracula')">ENHYPEN</button>
    </div>

  <!-- Script -->
  <script>
    function nextSlide() {
      document.getElementById('slide1').classList.remove('active');
      document.getElementById('slide2').classList.add('active');
    }

    function chooseGroup(group) {
      if (group === 'witch') {
        window.location.href = 'Witch.html'; // ganti dengan halaman pertanyaan princess
      } else if (group === 'dracula') {
        window.location.href = 'DraculaHunter.html'; // ganti dengan halaman pertanyaan vampire
      }
    }
  </script>

</body>
</html>

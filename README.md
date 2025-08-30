<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Happy Birthday Muskan</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      text-align: center;
      overflow: hidden;
    }
    .page {
      display: none;
      height: 100vh;
      padding: 40px;
      position: relative;
    }
    .active {
      display: block;
    }
    h1, h2 {
      margin-top: 50px;
    }
    .btn {
      display: inline-block;
      margin-top: 30px;
      padding: 15px 40px;
      background: #ff4081;
      color: white;
      font-size: 22px;
      border-radius: 50px;
      text-decoration: none;
      cursor: pointer;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
      transition: 0.3s;
    }
    .btn:hover {
      background: #e91e63;
      transform: scale(1.1);
    }

    /* Backgrounds */
    #page1 { background: linear-gradient(to right, #ffdde1, #ee9ca7); }
    #page2 { background: linear-gradient(to right, #a1c4fd, #c2e9fb); }
    #page4 { background: linear-gradient(to right, #fbc2eb, #a6c1ee); }
    #page5 { background-size: cover; background-position: center; }

    /* Cake with rainbow */
    .cake {
      margin-top: 40px;
      font-size: 100px;
      position: relative;
      display: inline-block;
    }
    .rainbow {
      width: 250px;
      height: 120px;
      border-radius: 50% 50% 0 0;
      background: conic-gradient(red, orange, yellow, green, blue, indigo, violet);
      margin: 0 auto;
      margin-bottom: -60px;
    }

    /* Balloons */
    .balloon {
      position: absolute;
      bottom: -120px;
      font-size: 45px;
      animation: float 6s infinite ease-in;
    }
    @keyframes float {
      0% { transform: translateY(0); opacity: 1; }
      100% { transform: translateY(-750px); opacity: 0; }
    }

    /* Pictures */
    .pics {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 20px;
      margin-top: 20px;
      justify-items: center;
    }
    .pics img {
      width: 220px;
      height: 220px;
      object-fit: cover;
      border-radius: 20px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.3);
      transition: 0.3s;
    }
    .pics img:hover {
      transform: scale(1.05);
    }

    /* Wish Styling */
    .wish {
      margin-top: 100px;
      font-size: 22px;
      color: #fff;
      font-style: italic;
      line-height: 1.8;
      max-width: 800px;
      margin-left: auto;
      margin-right: auto;
      background: rgba(0, 0, 0, 0.5);
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.3);
    }
    .wish strong {
      color: #ffccff;
      font-size: 26px;
    }
  </style>
</head>
<body>

  <!-- Page 1 -->
  <div class="page active" id="page1">
    <h1>🎂 Happy Birthday Muskan 🎉</h1>
    <a class="btn" onclick="nextPage(2)">Let's Start</a>
  </div>

  <!-- Page 2 (Cake + Rainbow + Balloons) -->
  <div class="page" id="page2">
    <h2>Here is your special Cake 🎂</h2>
    <div class="rainbow"></div>
    <div class="cake">🎂🕯🕯🕯</div>

    <!-- Balloons -->
    <div class="balloon" style="left:10%; animation-delay:0s;">🎈</div>
    <div class="balloon" style="left:25%; animation-delay:2s;">🎉</div>
    <div class="balloon" style="left:40%; animation-delay:1s;">🎈</div>
    <div class="balloon" style="left:55%; animation-delay:3s;">🎉</div>
    <div class="balloon" style="left:70%; animation-delay:1.5s;">🎈</div>
    <div class="balloon" style="left:85%; animation-delay:2.5s;">🎉</div>

    <a class="btn" onclick="nextPage(3)">Next 🎈</a>
  </div>

  <!-- Page 3 (Background Video) -->
  <div class="page" id="page3" style="position:relative; overflow:hidden;">

    <!-- Background Video -->
    <video autoplay muted loop playsinline
      style="position:absolute; top:0; left:0; width:100%; height:100%; object-fit:cover; z-index:-1;">
      <source src="muskan.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>

    <!-- Foreground Content -->
    <div style="position:relative; z-index:1; color:white; text-shadow:2px 2px 8px rgba(0,0,0,0.8);">
      <h2>🎥 A Special Surprise 🎉</h2>
      <p>Enjoy your day with this little magic ❤</p>
      <a class="btn" onclick="nextPage(4)">Next ❤</a>
    </div>
  </div>

  <!-- Page 4 (Pictures only) -->
  <div class="page" id="page4">
    <h2>🌟 Some Beautiful Memories 🌟</h2>
    <div class="pics">
      <img src="muskan1.jpg" alt="Memory 1">
      <img src="muskan2.jpg" alt="Memory 2">
      <img src="muskan3.jpg" alt="Memory 3">
      <img src="muskan4.jpg" alt="Memory 4">
    </div>
    <a class="btn" onclick="nextPage(5)">Next ➡ Wish</a>
  </div>

  <!-- Page 5 (Wish with custom background image) -->
  <div class="page" id="page5" style="background-image: url('muskan5.jpg');">
    <div class="wish">
      💌 <strong>Happy Birthday My Bhabhi, Muskan! 🎉❤</strong><br><br>
      Aaj ka din tumhari zindagi ka sabse khaas din hai,<br>
      aur meri dua hai ke tumhari zindagi hamesha khushiyon se bhari rahe. 🌸<br><br>
      Tum meri duaon ka woh hissa ho jo kabhi adhoora nahi hota,<br>
      meri muskaan ka woh sabab ho jo kabhi khatam nahi hota. 💕<br><br>
      Allah tumhari zindagi mein hamesha barkat aur mohabbat bhar de,<br>
      tumhari har dua qubool ho, aur tumhari har muskaan hamesha qayam rahe. ✨<br><br>
      Tum meri duniya ka sabse khoobsurat tohfa ho…<br>
      Aur meri zindagi ka sabse pyara hissaa bhi. 💖<br><br>
      <strong>I love you forever… Happy Birthday Muskan! 🎂🎈</strong>
    </div>
  </div>

  <script>
    function nextPage(num) {
      document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
      document.getElementById('page' + num).classList.add('active');
    }
  </script>

</body>
</html>

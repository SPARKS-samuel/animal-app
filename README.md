<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Animal Explorer</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Helvetica, sans-serif;
    }

    #header {
      position: fixed;
      top: 0;
      width: 100%;
      height: 80px;
      background-image: url('images/wood-bg.png');
      background-repeat: repeat-x;
      z-index: 1000;
    }

    #header img {
      display: block;
      margin: auto;
      height: 70%;
      padding-top: 15px;
    }

    #tabs-top, #tabs-bottom {
      position: fixed;
      width: 100%;
      height: 40px;
      background-color: forestgreen;
      z-index: 999;
    }

    #tabs-top {
      top: 80px;
    }

    #tabs-bottom {
      bottom: 0;
    }

    #tabs-top a, #tabs-bottom a {
      float: left;
      display: block;
      width: 33%;
      height: 40px;
      line-height: 40px;
      color: white;
      text-align: center;
      text-decoration: none;
      font-weight: bold;
    }

    #tabs-bottom a {
      width: 50%;
    }

    #main {
      margin-top: 120px;
      margin-bottom: 50px;
      background: url('images/map-blur.png') repeat-y;
      padding: 10px;
    }

    .info-box {
      display: flex;
      align-items: center;
      justify-content: space-between;
      background: rgba(255, 225, 55, 0.85);
      margin: 12px auto;
      padding: 10px;
      width: 90%;
      max-width: 500px;
      text-decoration: none;
      border-radius: 8px;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .info-box:hover {
      transform: scale(1.02);
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
    }

    .info-box img {
      height: 70px;
      width: 70px;
      object-fit: cover;
      border-radius: 50%;
      margin-right: 10px;
    }

    .info-box .right {
      height: 30px;
      margin-left: auto;
    }

    .info-box h3 {
      margin: 0;
      font-size: 1.1em;
      color: #572800;
    }

    .info-box p {
      margin: 2px 0 0 0;
      color: #131313;
      font-size: 0.9em;
    }

    .info-text {
      flex: 1;
    }

    @media (max-width: 600px) {
      .info-box {
        flex-direction: column;
        align-items: flex-start;
        text-align: left;
      }

      .info-box img {
        margin-bottom: 10px;
      }

      .info-box .right {
        align-self: flex-end;
        margin-top: 10px;
      }
    }
  </style>
</head>
<body>

<div id="header">
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/18/Nature_logo.png" alt="Animal Explorer Logo">
</div>

<div id="tabs-top">
  <a href="#">ANIMALS</a>
  <a href="#">MAP</a>
  <a href="#">PLACES</a>
</div>

<div id="main">
  <!-- Animal Cards -->
  <a class="info-box" href="details/elephants.html">
    <img src="https://upload.wikimedia.org/wikipedia/commons/3/37/African_Bush_Elephant.jpg" alt="Elephant">
    <div class="info-text">
      <h3>ELEPHANTS</h3>
      <p>Gentle giants of the jungle</p>
    </div>
    <img class="right" src="https://upload.wikimedia.org/wikipedia/commons/7/70/Arrow_right_font_awesome.svg" alt="Next">
  </a>

  <a class="info-box" href="details/giraffes.html">
    <img src="https://upload.wikimedia.org/wikipedia/commons/9/9f/Giraffe_standing.jpg" alt="Giraffe">
    <div class="info-text">
      <h3>GIRAFFES</h3>
      <p>Our giraffes love company</p>
    </div>
    <img class="right" src="https://upload.wikimedia.org/wikipedia/commons/7/70/Arrow_right_font_awesome.svg" alt="Next">
  </a>

  <a class="info-box" href="details/koalas.html">
    <img src="https://upload.wikimedia.org/wikipedia/commons/b/bb/Koala_climbing_tree.jpg" alt="Koala">
    <div class="info-text">
      <h3>KOALAS</h3>
      <p>Come take a look at the cute koalas</p>
    </div>
    <img class="right" src="https://upload.wikimedia.org/wikipedia/commons/7/70/Arrow_right_font_awesome.svg" alt="Next">
  </a>

  <a class="info-box" href="details/monkeys.html">
    <img src="https://upload.wikimedia.org/wikipedia/commons/f/f2/Capuchin_Costa_Rica.jpg" alt="Monkey">
    <div class="info-text">
      <h3>MONKEYS</h3>
      <p>Playful monkeys are cleverer than you think</p>
    </div>
    <img class="right" src="https://upload.wikimedia.org/wikipedia/commons/7/70/Arrow_right_font_awesome.svg" alt="Next">
  </a>

  <a class="info-box" href="details/pandas.html">
    <img src="https://upload.wikimedia.org/wikipedia/commons/0/0f/Grosser_Panda.JPG" alt="Panda">
    <div class="info-text">
      <h3>PANDAS</h3>
      <p>The pandas seem to be everyone's favorite</p>
    </div>
    <img class="right" src="https://upload.wikimedia.org/wikipedia/commons/7/70/Arrow_right_font_awesome.svg" alt="Next">
  </a>

  <a class="info-box" href="details/lions.html">
    <img src="https://upload.wikimedia.org/wikipedia/commons/7/73/Lion_waiting_in_Namibia.jpg" alt="Lion">
    <div class="info-text">
      <h3>LIONS</h3>
      <p>The king of the jungle awaits your visit</p>
    </div>
    <img class="right" src="https://upload.wikimedia.org/wikipedia/commons/7/70/Arrow_right_font_awesome.svg" alt="Next">
  </a>

  <a class="info-box" href="details/gemsboks.html">
    <img src="https://upload.wikimedia.org/wikipedia/commons/3/3f/Oryx_gazella_%28Namibia%29.jpg" alt="Gemsbok">
    <div class="info-text">
      <h3>GEMSBOKS</h3>
      <p>Come and see the majestic Gemsbok</p>
    </div>
    <img class="right" src="https://upload.wikimedia.org/wikipedia/commons/7/70/Arrow_right_font_awesome.svg" alt="Next">
  </a>

  <a class="info-box" href="details/gorillas.html">
    <img src="https://upload.wikimedia.org/wikipedia/commons/d/d9/Gorilla_%28Gorilla_gorilla_gorilla%29_male.jpg" alt="Gorilla">
    <div class="info-text">
      <h3>GORILLAS</h3>
      <p>Kong the gorilla is much friendlier than he looks</p>
    </div>
    <img class="right" src="https://upload.wikimedia.org/wikipedia/commons/7/70/Arrow_right_font_awesome.svg" alt="Next">
  </a>

  <a class="info-box" href="details/warthogs.html">
    <img src="https://upload.wikimedia.org/wikipedia/commons/b/b7/Phacochoerus_aethiopicus.jpg" alt="Warthog">
    <div class="info-text">
      <h3>WARTHOGS</h3>
      <p>Find out more about this fascinating creature</p>
    </div>
    <img class="right" src="https://upload.wikimedia.org/wikipedia/commons/7/70/Arrow_right_font_awesome.svg" alt="Next">
  </a>
</div>

<div id="tabs-bottom">
  <a href="#">WEATHER</a>
  <a href="#">FEEDBACK</a>
</div>

</body>
</html>

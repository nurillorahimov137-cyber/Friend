https://nurillorahimov137-cyber.github.io/Friend/ <!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="theme-color" content="#120b24">

  <title>Yangi xabar 💌</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;

      font-family:
        Inter,
        -apple-system,
        BlinkMacSystemFont,
        "Segoe UI",
        sans-serif;

      color: #fff;

      background:
        radial-gradient(circle at 20% 20%, #6d35b8 0%, transparent 30%),
        radial-gradient(circle at 80% 80%, #b43fd2 0%, transparent 28%),
        linear-gradient(135deg, #090613, #170b2d 50%, #0b0716);
    }

    /* -------------------------
       YULDUZCHALAR
    ------------------------- */

    .stars {
      position: fixed;
      inset: 0;
      pointer-events: none;
      overflow: hidden;
    }

    .star {
      position: absolute;
      width: 3px;
      height: 3px;
      border-radius: 50%;
      background: white;
      opacity: .5;
      animation: twinkle 3s infinite ease-in-out;
    }

    @keyframes twinkle {
      0%, 100% {
        opacity: .15;
        transform: scale(.7);
      }

      50% {
        opacity: .9;
        transform: scale(1.4);
      }
    }

    /* -------------------------
       ASOSIY KARTA
    ------------------------- */

    .card {
      position: relative;
      z-index: 2;

      width: min(92%, 430px);
      padding: 36px 28px;

      text-align: center;

      border: 1px solid rgba(255,255,255,.15);
      border-radius: 28px;

      background:
        linear-gradient(
          145deg,
          rgba(255,255,255,.13),
          rgba(255,255,255,.04)
        );

      backdrop-filter: blur(22px);
      -webkit-backdrop-filter: blur(22px);

      box-shadow:
        0 30px 80px rgba(0,0,0,.45),
        inset 0 1px rgba(255,255,255,.15);

      animation: cardAppear 1s ease;
    }

    @keyframes cardAppear {
      from {
        opacity: 0;
        transform: translateY(30px) scale(.96);
      }

      to {
        opacity: 1;
        transform: translateY(0) scale(1);
      }
    }

    /* -------------------------
       ICON
    ------------------------- */

    .icon {
      width: 76px;
      height: 76px;

      margin: 0 auto 22px;

      display: flex;
      align-items: center;
      justify-content: center;

      border-radius: 24px;

      font-size: 34px;

      background:
        linear-gradient(
          135deg,
          rgba(214,146,255,.35),
          rgba(145,74,255,.2)
        );

      border: 1px solid rgba(255,255,255,.15);

      box-shadow:
        0 10px 35px rgba(156,80,255,.25);

      animation: floating 3s ease-in-out infinite;
    }

    @keyframes floating {
      0%, 100% {
        transform: translateY(0);
      }

      50% {
        transform: translateY(-7px);
      }
    }

    /* -------------------------
       TEXT
    ------------------------- */

    .small {
      font-size: 12px;
      letter-spacing: 2px;
      text-transform: uppercase;
      color: rgba(255,255,255,.55);

      margin-bottom: 10px;
    }

    h1 {
      font-size: 28px;
      line-height: 1.25;

      margin-bottom: 14px;

      background:
        linear-gradient(
          90deg,
          #fff,
          #e4baff,
          #fff
        );

      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .description {
      color: rgba(255,255,255,.7);
      font-size: 15px;
      line-height: 1.7;

      margin-bottom: 28px;
    }

    /* -------------------------
       DEVELOPER STATUS
    ------------------------- */

    .developer {
      display: inline-flex;
      align-items: center;
      gap: 8px;

      margin-bottom: 25px;

      padding: 7px 12px;

      border-radius: 50px;

      background: rgba(0,0,0,.2);
      border: 1px solid rgba(255,255,255,.08);

      color: rgba(255,255,255,.55);

      font-family: monospace;
      font-size: 11px;
    }

    .online {
      width: 7px;
      height: 7px;

      border-radius: 50%;

      background: #8cffc1;

      box-shadow: 0 0 12px #8cffc1;
    }

    /* -------------------------
       BUTTONLAR
    ------------------------- */

    .buttons {
      position: relative;

      display: flex;
      gap: 10px;

      justify-content: center;
    }

    button {
      border: none;
      cursor: pointer;

      font-size: 14px;
      font-weight: 600;

      padding: 13px 20px;

      border-radius: 14px;

      transition:
        transform .25s,
        box-shadow .25s,
        background .25s;
    }

    .yes {
      color: #fff;

      background:
        linear-gradient(
          135deg,
          #9a5cff,
          #d45cff
        );

      box-shadow:
        0 10px 25px rgba(174,76,255,.3);
    }

    .yes:hover {
      transform: translateY(-3px);

      box-shadow:
        0 15px 35px rgba(174,76,255,.5);
    }

    .no {
      color: rgba(255,255,255,.75);

      background: rgba(255,255,255,.08);

      border: 1px solid rgba(255,255,255,.1);
    }

    .no:hover {
      background: rgba(255,255,255,.12);
    }

    /* -------------------------
       JAVOB EKRANI
    ------------------------- */

    .result {
      display: none;

      animation: resultAppear .7s ease;
    }

    @keyframes resultAppear {
      from {
        opacity: 0;
        transform: scale(.9);
      }

      to {
        opacity: 1;
        transform: scale(1);
      }
    }

    .result-icon {
      font-size: 48px;

      margin-bottom: 15px;

      animation: pop .7s ease;
    }

    @keyframes pop {
      0% {
        transform: scale(0);
      }

      70% {
        transform: scale(1.2);
      }

      100% {
        transform: scale(1);
      }
    }

    .message {
      color: rgba(255,255,255,.75);

      line-height: 1.8;
      font-size: 15px;

      margin: 15px 0 25px;
    }

    .telegram {
      display: inline-flex;
      align-items: center;
      justify-content: center;

      padding: 13px 22px;

      color: white;
      text-decoration: none;

      border-radius: 14px;

      background: linear-gradient(
        135deg,
        #7c5cff,
        #a855f7
      );

      box-shadow:
        0 10px 30px rgba(124,92,255,.3);

      transition: .25s;
    }

    .telegram:hover {
      transform: translateY(-3px);
      box-shadow:
        0 15px 40px rgba(124,92,255,.5);
    }

    /* -------------------------
       KONFETTI
    ------------------------- */

    .confetti {
      position: fixed;

      width: 8px;
      height: 8px;

      top: -10px;

      z-index: 10;

      animation:
        fall linear forwards;
    }

    @keyframes fall {
      to {
        transform:
          translateY(110vh)
          rotate(720deg);

        opacity: 0;
      }
    }

    /* -------------------------
       MOBIL
    ------------------------- */

    @media (max-width: 480px) {

      .card {
        padding: 30px 22px;
      }

      h1 {
        font-size: 25px;
      }

      .description {
        font-size: 14px;
      }

      .buttons {
        flex-direction: column;
      }

      button {
        width: 100%;
      }
    }
  </style>
</head>

<body>

  <!-- Yulduzchalar -->
  <div class="stars" id="stars"></div>


  <!-- Asosiy karta -->
  <main class="card">

    <!-- Boshlang'ich ekran -->
    <section id="mainScreen">

      <div class="icon">
        💌
      </div>

      <div class="small">
        Yangi bildirishnoma
      </div>

      <h1>
        Sizga kichik<br>
        bir taklif bor...
      </h1>

      <p class="description">
        Bu oddiy reklama emas 😄<br>
        Shunchaki siz bilan tanishishni
        istagan bir inson bor.
      </p>

      <div class="developer">
        <span class="online"></span>
        developer.exe — online
      </div>

      <div class="buttons">

        <button class="yes" onclick="accept()">
          🌷 Ha, nega emas?
        </button>

        <button class="no" id="noButton" onclick="decline()">
          🙈 Keyinroq
        </button>

      </div>

    </section>


    <!-- Natija -->
    <section class="result" id="result">

      <div class="result-icon">
        ✨
      </div>

      <div class="small">
        Connection established
      </div>

      <h1>
        Ajoyib! 😊
      </h1>

      <p class="message">
        Assalomu alaykum 🌷
        <br><br>

        Men siz bilan hali tanish emasman.
        Lekin oddiygina “Salom” deb yozish
        juda zerikarli tuyuldi 😄
        <br><br>

        Shuning uchun dasturchilik
        qobiliyatimdan foydalanib,
        sizga kichkina narsa tayyorladim.
        <br><br>

        Maqsadim oddiy:
        <b>yaxshi suhbatdosh va yangi do‘st topish.</b> 💜
        <br><br>

        Balki bu kichik sahifa
        tanishuvimizning birinchi sahifasidir? 😊
      </p>

      <!-- TELEGRAM USERNAME'NI O'ZGARTIR -->
      <a
        class="telegram"
        href="https://t.me/YOUR_USERNAME"
        target="_blank"
      >
        💬 Telegramda salomlashamiz
      </a>

    </section>

  </main>


  <script>

    /* -------------------------
       YULDUZCHALAR YARATISH
    ------------------------- */

    const stars = document.getElementById("stars");

    for (let i = 0; i < 70; i++) {

      const star = document.createElement("div");

      star.className = "star";

      star.style.left =
        Math.random() * 100 + "%";

      star.style.top =
        Math.random() * 100 + "%";

      star.style.animationDelay =
        Math.random() * 3 + "s";

      star.style.animationDuration =
        (2 + Math.random() * 3) + "s";

      stars.appendChild(star);
    }


    /* -------------------------
       HA BOSILGANDA
    ------------------------- */

    function accept() {

      const mainScreen =
        document.getElementById("mainScreen");

      const result =
        document.getElementById("result");

      mainScreen.style.display = "none";

      result.style.display = "block";

      createConfetti();
    }


    /* -------------------------
       KEYINROQ BOSILGANDA
    ------------------------- */

    function decline() {

      const button =
        document.getElementById("noButton");

      const messages = [
        "Hali o‘ylab ko‘ring 😄",
        "Shoshilmang 🙈",
        "Balki bir imkoniyat berarsiz? 😁",
        "Men yaxshi odamman-ku 😂"
      ];

      const random =
        messages[Math.floor(
          Math.random() * messages.length
        )];

      button.innerText = random;

      button.style.position = "relative";

      button.style.transform =
        `translate(
          ${(Math.random() * 40) - 20}px,
          ${(Math.random() * 20) - 10}px
        )`;
    }


    /* -------------------------
       KONFETTI
    ------------------------- */

    function createConfetti() {

      const symbols = [
        "💜",
        "✨",
        "🌷",
        "💫",
        "💗"
      ];

      for (let i = 0; i < 35; i++) {

        const confetti =
          document.createElement("div");

        confetti.className = "confetti";

        confetti.innerText =
          symbols[
            Math.floor(
              Math.random() * symbols.length
            )
          ];

        confetti.style.left =
          Math.random() * 100 + "vw";

        confetti.style.fontSize =
          (10 + Math.random() * 15) + "px";

        confetti.style.animationDuration =
          (2 + Math.random() * 3) + "s";

        confetti.style.animationDelay =
          Math.random() * .7 + "s";

        document.body.appendChild(confetti);

        setTimeout(() => {
          confetti.remove();
        }, 5000);
      }
    }

  </script>

</body>
</html>

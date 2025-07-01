---
layout: default
theme: jekyll-theme-minimal
title: Chest of godness homepage
description: Bookmark this to keep an eye on my project updates
---!
<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta property="og:title" content="Скриня добра">
  <meta property="og:description" content="Відкрий скарб добра, підтримай нас ще раз">
  <meta property="og:image" content="https://example.com/images/home.png">
  <meta property="og:url" content="https://example.com">
  <link href="https://fonts.googleapis.com/css2?family=Manrope:wght@600&family=Geologica:wght@700&display=swap" rel="stylesheet">
  <style>
    * { box-sizing: border-box; }

    html, body {
      margin: 0;
      padding: 0;
      width: 100%;
      height: 100%;
      font-family: 'Manrope', sans-serif;
      background-color: #FFFFE3;
      overflow-x: hidden;
      scroll-behavior: smooth;
    }

    body {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }

    .top-text, .top-caption, .center-caption, .last-caption {
      margin-top: 70px;
      padding: 20px;
      font-weight: 600;
      font-size: 70px;
      color: #243a57;
    }

    .center-caption {
      font-size: 70px;
      text-align: center;
      opacity: 1;
      transition: opacity 0.5s ease-in-out;
      margin-top: 20px;
    }

    .top-caption {
      font-size: 70px;
      margin-top: 400px;
      color: #243a57;
    }

    .last-caption {
      font-size: 70px;
      margin-top: 400px;
      color: #243a57;
    }

    .logos {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 80px;
      margin-bottom: 30px;
      flex-wrap: wrap;
    }

    .logos img {
      max-width: 700px;
      height: auto;
    }

    .center-image {
      width: 70%;
      max-height: 150vh;
      height: auto;
      margin-top: -10px;
      margin-bottom: 15px;
      z-index: 1;
    }

    .cdaka-image {
      width: 30%;
      max-height: 150vh;
      height: auto;
      margin-top: -50px;
      margin-bottom: 15px;
      z-index: 1;
    }

    .button-wrapper { margin-top: 50px; }

    .wave-button, .help-button {
      position: relative;
      display: inline-block;
      padding: 38px 80px;
      color: white;
      text-transform: uppercase;
      letter-spacing: 2px;
      font-size: 34px;
      overflow: hidden;
      transition: 0.2s;
      background: rgba(36, 58, 87, 1);
      border-radius: 50px;
      cursor: pointer;
      border: none;
      z-index: 10;
    }

    .wave-button:hover, .help-button:hover {
      box-shadow: 0 0 20px rgba(36, 58, 87, 1), 0 0 60px rgba(36, 58, 87, 1), 0 0 100px rgba(36, 58, 87, 1);
      transition-delay: 0.1s;
    }

    .two {
      display: none;
      opacity: 0;
      transition: opacity 1s ease-in-out;
      margin-bottom: 100px;
    }

    .fly-container {
      position: relative;
      width: 100%;
      max-height: 400px;
      overflow: hidden;
      margin: 0 auto;
    }

    .final-row {
      display: flex;
      justify-content: center;
      align-items: flex-start;
      gap: 40px;
      flex-wrap: wrap;
    }

    .fly-item {
      width: 300px;
      height: 300px;
      margin-top: 100px;
      margin-bottom: 700px;
      background-size: contain;
      background-repeat: no-repeat;
      background-position: center;
      opacity: 0;
      transform: translateY(200px);
      transition: all 0.8s ease;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .fly-text {
      position: absolute;
      top: 40px;
      left: 50%;
      transform: translateX(-50%);
      font-size: 24px;
      font-weight: bold;
      color: #333;
      opacity: 0;
      transition: opacity 1s ease;
      z-index: 10;
    }

    .fly-in { opacity: 1; transform: translateY(0); }

    .text-in { opacity: 1; }

    .tree {
      display: none;
      opacity: 0;
      transition: opacity 0.5s ease-in-out;
      margin-bottom: 200px;
    }

    .helpbutton-wrapper { margin-top: 50px; }

    .qr {
      width: 80%;
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      max-width: 600px;
      height: auto;
      display: inline-block;
      margin: 73px 30px;
    }

    /* === Адаптація для мобільних === */
    @media (max-width: 768px) {
      .top-text, .top-caption, .center-caption, .last-caption {
        font-size: 28px;
        margin-top: 40px;
        padding: 10px;
      }

      .logos {
        gap: 20px;
        flex-direction: column;
        justify-content: center;
        align-items: center;
      }

      .logos img { max-width: 90%; }

      .center-image { width: 90%; }

      .cdaka-image {
        width: 70%;
        margin-top: 0;
      }

      .button-wrapper { margin-top: 10px; }

      .wave-button, .help-button {
        padding: 20px 40px;
        font-size: 18px;
      }

      .final-row { gap: 20px; }

      .fly-item {
        width: 80px;
        height: 80px;
        margin-top: 50px;
        margin-bottom: 200px;
      }

      .fly-text {
        font-size: 16px;
        top: 20px;
      }

      .qr {
        width: 80%;
        margin: 40px 20px;
      }

      .two { margin-bottom: -150px; }

      .tree { margin-bottom: 100px; }
    }
  </style>
</head>
<body>

<!-- ПЕРЕКЛАДАЧ -->
<div id="google_translate_element" style="position: absolute; top: 10px; right: 10px; z-index: 9999;"></div>

<audio id="myAudio">
  <source src="./audio/hava-nagila-orchestra-clarinet-7671.mp3" type="audio/mpeg">
  Ваш браузер не підтримує аудіо.
</audio>

<section class="one">
  <div class="top-text">Кожен акт добра — це промінь світла у нашому світі</div>
  <div class="logos">
    <a href="https://www.instagram.com/mazal.tov.zp/" target="_blank">
      <img src="./images/mazal.png" alt="Mazal Tov Logo">
    </a>
    <a href="https://www.facebook.com/HesedMichael.zp.ua/?locale=ru_RU" target="_blank">
      <img src="./images/bluelogo 1.png" alt="Хесед Міхаель Logo">
    </a>
  </div>

  <img src="./images/home.png" alt="Дім" class="center-image">

  <div class="button-wrapper">
    <button class="wave-button">ВІДКРИТИ СКАРБ ЦДАКИ</button>
  </div>
</section>

<section class="two">
  <div class="top-caption">
    Завдяки вашій цдаці ми створюємо безпеку, силу <br> громади та майбутнє для кожного
  </div>
  <img src="./images/cdaka.png" alt="Цдака" class="cdaka-image">
  <div class="center-caption"></div>
  <div class="fly-container"></div>
</section>

<section class="tree">
  <div class="last-caption">
    Нехай ваша доброта повернеться до вас <br> сторицею — תִּזְכּוּ לְמִצְווֹת (тизку ле-міцвот).
  </div>
  <div class="helpbutton-wrapper">
    <a href="https://next.privat24.ua/payments/form/%7B%22token%22%3A%22be0ba580-a488-4ab6-b285-4fe127c71313%22%7D" target="_blank">
      <button class="help-button">ПІДТРИМАТИ ЩЕ РАЗ</button>
    </a>
  </div>

  <a href="https://www.facebook.com/JCCMazalTov/?locale=ru_RU" target="_blank">
    <img src="./images/qrmazal.png" alt="QR-код Mazal" class="qr">
  </a>
  <a href="https://next.privat24.ua/payments/form/%7B%22token%22%3A%22be0ba580-a488-4ab6-b285-4fe127c71313%22%7D" target="_blank">
    <img src="./images/qrhesed.png" alt="QR-код Hesed" class="qr">
  </a>
</section>

<script>
document.addEventListener("DOMContentLoaded", () => {
  const button = document.querySelector('.wave-button');
  const sectionTwo = document.querySelector('.two');
  const container = document.querySelector('.fly-container');
  const caption = document.querySelector('.center-caption');
  const treeSection = document.querySelector('.tree');
  const items = [
    { img: './images/coin.png' },
    { img: './images/dove.png' },
    { img: './images/candle.png' },
    { img: './images/scroll.png' }
  ];
  const texts = [
    '«Слова світла, що розпалюють серця»',
    '«Пам’ятаємо. Дякуємо. Надихаємося»',
    '«Кожен вчинок — іскра добра»',
    '«Нехай доброта живе у вічності»'
  ];
  let animationStarted = false;
  const audio = document.getElementById('myAudio');

  function animateCaptionText() {
    let index = 0;
    function changeText() {
      caption.style.opacity = '0';
      setTimeout(() => {
        caption.textContent = texts[index];
        caption.style.opacity = '1';
        index++;
        if (index < texts.length) {
          setTimeout(changeText, 2000);
        } else {
          setTimeout(() => {
            treeSection.style.display = 'block';
            setTimeout(() => {
              treeSection.style.opacity = '1';
              treeSection.scrollIntoView({ behavior: 'smooth' });
            }, 50);
          }, 3000);
        }
      }, 500);
    }
    changeText();
  }

  button.addEventListener('click', () => {
    if (animationStarted) return;
    animationStarted = true;
    if (audio) {
      audio.currentTime = 0;
      audio.play();
    }
    sectionTwo.style.display = 'block';
    setTimeout(() => {
      sectionTwo.style.opacity = '1';
      sectionTwo.scrollIntoView({ behavior: 'smooth' });
    }, 100);
    container.innerHTML = '';
    const row = document.createElement('div');
    row.className = 'final-row';
    container.appendChild(row);
    let delay = 0;
    items.forEach((item) => {
      const wrapper = document.createElement('div');
      wrapper.className = 'fly-item';
      wrapper.style.backgroundImage = `url('${item.img}')`;
      row.appendChild(wrapper);
      setTimeout(() => {
        wrapper.classList.add('fly-in');
      }, delay);
      delay += 1200;
    });
    animateCaptionText();
  });
});
</script>
<script type="text/javascript">
  function googleTranslateElementInit() {
    new google.translate.TranslateElement({
      pageLanguage: 'uk',
      includedLanguages: 'uk,en,he,ru',
      layout: google.translate.TranslateElement.InlineLayout.SIMPLE
    }, 'google_translate_element');
  }
</script>
<script type="text/javascript" 
  src="//translate.google.com/translate_a/element.js?cb=googleTranslateElementInit">
</script>

</body>
</html>

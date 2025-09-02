<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Случайная картинка и текст</title>
  <style>
    body { font-family: sans-serif; text-align: center; margin-top: 50px; }
    img { max-width: 600px; margin-top: 20px; }
    #text { margin-top: 10px; font-size: 18px; }
  </style>
</head>
<body>
      <a href="#" onclick="window.open('file:///C:/Users/Asus/SCripts%20Visual/script%201.html'); return false">CLICK ME</a>
  <h1>ZXC ROLL 🎲</h1>
  <button onclick="showRandom()">Показать случайное</button>

  <div id="output">
    <img id="image" src="" alt="" style="display:none;">
    <div id="text"></div>
  </div>

  <script>
    const items = [
      { img: "https://i.pinimg.com/736x/5a/89/6c/5a896cc81d79be709cdfd4b7b75cf354.jpg", text: " ХЫВАХЗВЫАХЗ ЕБАТЬ ТЫ ДАЛБАЕБ НЕ ВЕЗУЧИЙ!" },
      { img: "https://image.noelshack.com/fichiers/2022/40/1/1664834297-jesuscerrr.png", text: " как же мне тебя жаль." },
      { img: "https://tse2.mm.bing.net/th/id/OIP.VygyMRUrFsohD3vd4OoBmQHaFP?cb=thfc1&rs=1&pid=ImgDetMain&o=7&rm=3", text: " Что-то загадочное..." },
      { img: "https://i.pinimg.com/originals/c8/68/6e/c8686e7562231e1ce32cc74a2d300224.jpg", text: " ну что ту тсказать, 10 репортов обеспечены" },
      { img: "https://i.pinimg.com/originals/0d/62/63/0d62632faf26197b275dac5239cc18b2.jpg", text: " Просто мемасик" }
    ];

    function showRandom() {
      const randomItem = items[Math.floor(Math.random() * items.length)];
      document.getElementById("image").src = randomItem.img;
      document.getElementById("image").style.display = "block";
      document.getElementById("text").textContent = randomItem.text;
    }
  </script>

</body>
</html>

# my-video-buttons
my-video-buttons
[сайт.txt](https://github.com/user-attachments/files/22951220/default.txt)
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Видео кнопки</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      background: linear-gradient(135deg, #667eea, #764ba2);
      font-family: 'Segoe UI', sans-serif;
      color: white;
      overflow: hidden;
    }

    h1 {
      font-size: 2.5em;
      margin-bottom: 40px;
      animation: fadeInDown 1s ease forwards;
    }

    .button-container {
      display: flex;
      gap: 30px;
    }

    button {
      position: relative;
      background: transparent;
      border: 2px solid white;
      color: white;
      font-size: 2em;
      padding: 20px 40px;
      border-radius: 15px;
      cursor: pointer;
      transition: all 0.4s ease;
      overflow: hidden;
      z-index: 1;
    }

    button::before {
      content: "";
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: white;
      z-index: -1;
      transition: all 0.4s ease;
    }

    button:hover::before {
      left: 0;
    }

    button:hover {
      color: #764ba2;
      transform: scale(1.1);
      box-shadow: 0 0 20px rgba(255, 255, 255, 0.6);
    }

    @keyframes fadeInDown {
      from { opacity: 0; transform: translateY(-30px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <h1>Выбери видео</h1>
  <div class="button-container">
    <button onclick="window.location.href='https://youtu.be/dQw4w9WgXcQ'">1</button>
    <button onclick="window.location.href='https://youtu.be/3JZ_D3ELwOQ'">2</button>
    <button onclick="window.location.href='https://youtu.be/oHg5SJYRHA0'">3</button>
  </div>
</body>
</html>

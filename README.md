# HW-8
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="./style/style.css">
    <title>Document</title>
</head>
<body>
    <div class="text-box">
        <h3>Пофарбуйте мене в рожевий колір (color:pink).</h3>
        <p>Даний елемент має залишитись неоформленим.</p>
        <p id="greycol">Пофарбуйте мене в сірий колір (color:grey).</p>
        <div>Даний елемент має залишитись неоформленим.</div>
        <div><p>Пофарбуйте мене в червоний колір (color:red).</p></div>
        <h3>Даний елемент має залишитись неоформленим.</h3>
        <p>Пофарбуйте мене в зелений колір (color:green).</p>
        <p class="yellow">Пофарбуйте мене в жовтий колір (color:yellow).</p>
      </div>
      <div class="lessons-container">
        <ul class="lessons monday">
          <li>Математика</li>
          <li>Фізика</li>
          <li>Хімія</li>
        </ul>
        <ul class="lessons tuesday">
          <li>Історія</li>
          <li>Література</li>
        </ul>
        <ul class="lessons wednesday">
          <li>Географія</li>
          <li>Біологія</li>
          <li>Мистецтво</li>
        </ul>
        <ul class="lessons thursday">
          <li>Економіка</li>
          <li>Правознавство</li>
        </ul>
        <ul class="lessons friday">
          <li>Фізкультура</li>
          <li>Інформатика</li>
          <li>Мова</li>
        </ul>
      </div>
</body>
</html>
# Style.css
.text-box h3:first-of-type {
    color: pink; /* Пофарбуйте мене в рожевий колір */
  }
  
  .text-box p :id-greycol{
    color: grey; /* Пофарбуйте мене в сірий колір */
  }

  .text-box div:last-of-type p {
    color: red; /* Пофарбуйте мене в червоний колір */
  }
  
  .text-box p:nth-of-type {
    color: green; /* Пофарбуйте мене в зелений колір */
  }
  
  .text-box .yellow {
    color: yellow; /* Пофарбуйте мене в жовтий колір */
  }
  
  /* Основний контейнер для уроків */
.lessons-container {
    display: flex;
    justify-content: space-around;
    margin-top: 20px;
  }
  
  /* Стилі для кожного списку уроків */
  .lessons {
    list-style-type: none;
    padding: 10px;
    width: 150px;
  }
  
  /* Понеділок */
  .monday li {
    background-color: #ffcccc;
  }
  
  /* Вівторок */
  .tuesday li {
    background-color: #ccffcc;
  }
  
  /* Середа */
  .wednesday li {
    background-color: #ccccff;
  }
  
  /* Четвер */
  .thursday li {
    background-color: #ffffcc;
  }
  
  /* П'ятниця */
  .friday li {
    background-color: #ffccff;
  }
  
  /* Псевдокласи стану */
  /* Перший елемент */
  .lessons li:first-child {
    border-top: 2px solid black;
  }
  
  /* Останній елемент */
  .lessons li:last-child {
    border-bottom: 2px solid black;
  }
  
  /* Елемент, який знаходиться під курсором */
  .lessons li:hover {
    transform: scale(1.1);
  }
  
  /* Активний елемент (при натисканні) */
  .lessons li:active {
    background-color: #ffa07a;
  }
  
  /* Відвідані посилання */
  .lessons li:visited {
    opacity: 0.6;
  }
  
  /* Структурні псевдокласи */
  /* Перший елемент списку */
  .lessons:first-of-type li {
    font-weight: bold;
  }
  
  /* Останній елемент списку */
  .lessons:last-of-type li {
    font-style: italic;
  }
  
  /* Непарні елементи */
  .lessons li:nth-child(odd) {
    transform: rotate(3deg);
  }
  
  /* Парні елементи */
  .lessons li:nth-child(even) {
    transform: rotate(-3deg);
  }
  

# html
<h1>Главный заголовок</h1>
<h2>Подзаголовок</h2>
<h3>Еще один уровень</h3>


<p>Это абзац текста. Он отображается как отдельный блок с отступом.</p>
<pre> это текст с любым расположением символов</pre>
<span> чтобы при переносе текста перенос произаводился целыми словами</span>

<ul>
  <li>p в стрелочных скобках это параграф </li>
  <li>h в стрелочных скобках это заголовок</li>
  <li>ul внутри которого li это маркированный список</li>
</ul>


<ul>
  <li><b> — простое выделение текста. Его можно использовать в любом месте для визуального выделения текста. Никакой смысловой нагрузки этот тег не несёт
  <li><strong> — логическое выделение важного участка текста. Этот тег несёт смысловую нагрузку и размечает именно важную часть. Его не следует применять на всех участках подряд
<ul>


<ul>
  <li>Тегом <i> было размечено название портала Code Basics. Тег предназначен для визуального выделение текста курсивом и не несёт смысловой нагрузки
  <li>Тегом <em> была выделена фраза «бесплатные курсы». Это логический акцент на бесплатности курсов, который был придан предложению. Курсов много, а бесплатных нет, поэтому стоит добавить акцент на эту часть предложения
<ul>



<ol>
  <li>это нумерованный список</li>
</ol>

"пример как создаются таблицы"

<table>
  <thead>
    <tr>
      <th>Фрукты</th>
      <th>Вес</th>
      <th>цена</th>
    </tr>
  </thead>
  
  <tbody>
    <tr>
      <td>apple</td>
      <td>100g</td>
      <td>1$</td>
    </tr>

    <tr>
      <td>banana</td>
      <td>150g</td>
      <td>1,2$</td>
    </tr>

    <tr>
      <td>pineapple</td>
      <td>1Kg</td>
      <td>10$</td>
    </tr>
  </tbody>
</table>


<table> — область таблицы
<tr> — строка
<thead> — шапка таблицы
<th> — ячейка шапки
<tbody> — тело таблицы
<td> — ячейка


"В таблице colspan объеденяет строки по горизонтали, а rowspan по горизонтали"


"пример ссылки"<a href="https://code-basics.com/">Перейти на сайт Code Basics</a>


<code>для кодов </code>

<img> для изображений alt если изображение не доступно


<audio>для встраивания аудио
<audio controls>
  <source src="https://example.com/audio.mp3">
  <source src="https://example.com/audio.ogg">
</audio>
<source>в котором указываются пути на другие форматы аудио файлов.

<video controls>
  <source src="https://example.com/our-video.mp4" type="video/mp4">
  <source src="https://example.com/our-video.webm" type="video/webm">
  <source src="https://example.com/our-video.ogg" type="video/ogg">
</video>


<video width="320" height="240" controls>
  <source src="https://www.w3schools.com/html/movie.mp4" type="video/mp4">
</video>

controls — Добавляет элементы управления для видеоплеера
autoplay — Автоматическое воспроизведение после загрузки видео
width — Ширина видеоплеера
height — Высота видеоплеера

не очень понял метатэги



rel для указания контента
href для указания ссылки на иконку

<link rel="icon" href="https://www.w3schools.com/favicon.ico" sizes="64x64">


width — ширина сайта. Указывается в пикселях. Возможно использование значения device-width для установки ширины страницы равной ширине устройства.
height — высота сайта. Указывается в пикселях. Возможно использование значения device-height для установки высоты страницы равной высоте устройства.
initial-scale — начальный коэффициент масштабирования. Может принимать значение от 0.1 до 10.0. Значение единица масштабирует страницу по умолчанию.
user-scalable — указывает, может ли пользователь масштабировать страницу, то есть приближать или отдалять её. Принимает значение yes и no


<meta name="viewport" content="width=device-width, initial-scale=1.0">

<form action="/people"></form>
Основным атрибутом у тега <form> является action — путь к файлу, где располагается обработчик данных. Именно туда уйдут данные после отправки формы.

ДЛЯ ВВОДА ДАННЫХ
<form>
  <label>Введите имя</label>
  <input type="text">
</form>

Чтобы помочь пользователю сориентироваться используется атрибут placeholder у тега <input>.
<form>
  <label for="name">Введите имя и фамилию</label>
  <input type="text" id="name" placeholder="Иван Иванов">
</form>


<form action="/people">
  <label for="pin">Введите пинкод</label>
  <input type="password" id="pin" placeholder="1234">
</form>
в input используется email
number
search
tel
url




чекбоксы
<form action="/people">
  <label>
    <input type="checkbox" name="fruits" value="apple">
    apple
  </label>
  <label>
    <input type="checkbox" name="fruits" value="pineapple">
    pineapple
  </label>
</form>


HTML: Радиокнопка
<form action="/people">
 <label>
  <input type="radio" name="delivery" value="yes">
  yes
 </label>
 <br>
 <label>
  <input type="radio" name="delivery" value="no">
  no
 </label>
</form>


HTML: Textarea
<form action="/people">
 <textarea rows="4" cols="30">
 </textarea>
</form>


HTML: Список
<form action="/people">
 <select>
  <option>apple</option>
  <option>pineapple</option>
  <option>banana</option>
 </select>
</form>



HTML: Отправка формы
    <label>
        Name
        <input type="text">
    </label>
    <label>
        Email
        <input type="text">
    </label>
    <select multiple>
        <option disabled>Which course you want to take?</option>
        <option>JS</option>
        <option>PHP</option>
        <option>Java</option>
    </select>

    <button>Apply</button>
</form>



HTML: Шапка
<header>
  <img src="https://i.imgur.com/g64f8to.png" alt="Логотип"> <!-- Логотип сайта -->
  <div id="menu"> <!-- Меню -->
    <ul>
      <li><a href="/">Главная</a></li>
      <li><a href="/about">О нас</a></li>
      <li><a href="/contacts">Контакты</a></li>
    </ul>
  </div>
</header>

HTML: Меню
<header>
  <img src="https://i.imgur.com/g64f8to.png" alt="Code Basics"> <!-- Логотип сайта -->
  <nav> <!-- Меню -->
    <ul>
      <li><a href="/">Главная</a></li>
      <li><a href="/about">О нас</a></li>
    </ul>
  </nav>
</header>


HTML: Уникальный контент страницы
<header>
  <img src="https://i.imgur.com/g64f8to.png" alt="Code Basics">
  <nav> <!-- Меню -->
    <ul>
      <li><a href="/">Главная</a></li>
      <li><a href="/about">О нас</a></li>
    </ul>
  </nav>
</header>

<main>
  <!-- Основной контент страницы. Это может быть статья, описание услуги, данные на странице, контакты, форма заказа услуги -->
</main>
main — уникальная секция, которая используется один раз на всю страницу

HTML: Секция
header>
    <img src="https://i.imgur.com/g64f8to.png" alt="Code Basics">
    <nav>
        <ul>
            <li><a href="/languages/html">HTML Course</a></li>
            <li><a href="/languages/css">CSS Course</a></li>
        </ul>
    </nav>
</header>

<main>
    <h1>Free hands-on programming courses for those starting from scratch</h1>
    <p>From the creators of Hexlet</p>

    <section>
        <h2>Languages available for learning</h2>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>Java</li>
            <li>Python</li>
            <li>Racket</li>
        </ul>
    </section>

    <section>
        <h2>Frontend courses</h2>
        <ul>
            <li>HTML</li>
            <li>CSS</li>
        </ul>
    </section>
</main>


для обозначения секции используется тег <article>. Он предназначается для разметки секции, которая может быть использована самостоятельно и не привязана структурно к конкретной странице.

HTML: Самостоятельная секция

<header>
  <img src="https://i.imgur.com/g64f8to.png" alt="Логотип">
  <nav>
    <ul>
      <li><a href="https://code-basics.com/ru/languages/html/lessons/article">Hello</a></li>
      <li><a href="https://code-basics.com/ru/languages/html/lessons/article">World</a></li>
    </ul>
<main>
  <section>
    <h2>Hello World!</h2>
    <article class="article-block">
      <h3>Usluga1</h3>
      <p>Описание новой услуги</p>
      <a href="https://code-basics.com/ru/languages/html/lessons/article">a</a>
    </article>
    <article class="article-block">
      <h3>Usluga2</h3>
      <p>Описание новой услуги</p>
      <a href="https://code-basics.com/ru/languages/html/lessons/article">b</a>
    </article>
  </section>
</main>


HTML: Боковая панель
Для того чтобы корректно разметить такую область, существует тег <aside>, внутри которого и располагается наша боковая панель.
<header>
  <img src="https://i.imgur.com/g64f8to.png" alt="Code Basics">
  <nav>
    <ul>
      <li><a href="https://code-basics.com/ru/languages/html/lessons/aside">Code</a></li>
      <li><a href="https://code-basics.com/ru/languages/html/lessons/aside">code2</a></li>
    </ul>
  </nav>
</header>
<aside>
  <nav>
    <ul>
      <li><a href="/service-1/">Услуга 1</a></li>
      <li><a href="/service-2/">Услуга 2</a></li>
    </ul>
  </nav>
</aside>

<main>
  <section class="title">
  <h2>Hello world!</h2>
  <section class="more">
  <article class="article-block">
    <h3>Услуга 1</h3>
    <p>Описание новой услуги</p>
    <a href="#">Ссылка на услугу</a>
  </article>
  <article class="article-block">
    <h3>Услуга 2</h3>
    <p>Описание новой услуги</p>
    <a href="#">Ссылка на услугу</a>
    </article>
  </section>

HTML: Семантический WEB
<main> <!-- Определение основной части страницы -->
  <article> <!-- Определение статьи -->
    <header> <!-- Заголовочная информация статьи -->
      <h1>Название статьи</h1>
      <img src="https://i.imgur.com/g64f8to.png" height="50" alt="Заголовок статьи">
    </header>

    <p>Текст нашей статьи</p>

    <footer> <!-- «Подвал статьи» с указанием автора и даты -->
      <address> <!-- Информация об авторе статьи -->
        <p>Автор: Pavel</p>
        <p>Email: gmail</p>
      </address>
      <time datetime="2025-05-18">18may</time> <!-- Дата написания статьи -->
    </footer>
  </article>
</main>







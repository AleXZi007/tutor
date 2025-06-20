Репетитор Код описание
Структура HTML
<!DOCTYPE html>
•	Объявляет тип документа, сообщает браузеру, что это HTML5.
<html lang="ru">
•	Корневой элемент страницы, язык — русский.
<head>
•	Содержит метаданные:
o	<meta charset="UTF-8"> — кодировка UTF-8.
o	<meta name="viewport" ...> — адаптивность для мобильных устройств.
o	<title> — заголовок страницы (отображается на вкладке браузера).
o	<link rel="stylesheet" href="styles.css"> — подключение внешнего CSS-файла.
<body>
•	Основное содержимое страницы.
<header>
•	Шапка сайта:
o	Логотип (<img src="logo.png" ...>)
o	Название ("Репетитор Алексей Иванов")
<section class="services">
•	Блок "Мои услуги":
o	Заголовок (<h2>)
o	Список услуг (<div class="service-list">), каждая услуга — отдельный <div class="service"> с картинкой, названием и описанием.
<section class="contact">
•	Контактная информация:
o	Телефон (ссылкой для звонка)
o	Email (ссылкой для отправки письма)
o	Адрес
<footer>
•	Подвал с копирайтом.
 
2. CSS (Стили)
body {
  font-family: Arial, sans-serif;
  margin: 0;
  background: #f4f4f9;
}

•	Основные настройки: шрифт, отсутствие отступов, светлый фон.
header, footer {
  background: #036;
  color: #fff;
  text-align: center;
  padding: 20px 0;
}
footer { padding: 10px 0; }

•	Шапка и подвал: синий фон, белый текст, выравнивание по центру, отступы.
.logo, .service img { width: 60px; }

•	Размер логотипа и иконок услуг.
h1 { margin: 10px 0 0; }

•	Отступы для основного заголовка.
.services, .contact {
  padding: 20px;
  text-align: center;
}

•	Внутренние отступы и выравнивание для секций "Услуги" и "Контакты".
.service-list {
  display: flex;
  justify-content: center;
  gap: 30px;
  margin-top: 20px;
}

•	Список услуг в виде горизонтального flex-контейнера с промежутками между карточками.
.service {
  background: #fff;
  padding: 15px;
  border-radius: 8px;
  width: 250px;
  box-shadow: 0 2px 4px rgba(0,0,0,.1);
}
.service img { margin-bottom: 10px; }

•	Оформление карточек услуг: белый фон, скругления, тень, фиксированная ширина, отступы.
.contact { background: #eef; }

•	Секция контактов с голубым фоном.
 
3. Кратко о назначении
•	HTML задаёт структуру: шапка, услуги, контакты, подвал.
•	CSS оформляет внешний вид: цвета, отступы, выравнивание, стили карточек.


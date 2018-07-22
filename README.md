<h2>How to use uniMail</h2>

<ol>
	<li>Include jQuery;</li>
	<li>Include Ajax code from script.js;</li>
	<li>Change Ajax selector in you JS;</li>
	<li>Create HTML form with you form class;</li>
	<li>Create HTML Hidden Required Fields with you values;</li>
	<li>Change path to mail.php in you JS.</li>
	<li>Done!</li>
</ol>

<p>Источник исходного скрипта: https://github.com/agragregra/uniMail</p>
<p>Иногда необходимо, чтобы после оформления заказа, пользователь перенаправлялся на страницу "Спасибо". Это делается для того, чтобы собрать аудиторию (ретаргетинг) и правильно выставить цели Яндекс.Метрики. Кроме того, на странице "Спасибо" можно разместить допродающее видео и акции (up-sell).</p>

<p>Итак, я добавил в файл script.js следующую строку:</p>

<p>window.location.href = "http://karriweb.ru";</p>

<p>Она осуществляет перенаправление по указанному пути, если заявка успешно отправилась.</p>

<p>Также Вам можетпригодится данный код:</p>

<p>if ($_SERVER['HTTP_REFERER'] != "http://domain.ru/index.php") {
   die();
}</p>

<p>С помощью него можно ограничить доступ  к странице "Спасибо", если переход осуществляется из адресной строки или с поисковых систем. Лучше вообще закрыть страницу "Спасибо" от индексации поисковыми системами.</p>
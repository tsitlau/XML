# XML
 21. Создать внешний репозиторий c названием XML.
В шапке сайта слева нажать +, выбрать New repository
В поле Repository name введите XML, выберите Public и Add a README file.
Нажать Create repository.

 22. Клонировать репозиторий XML на локальный компьютер.
Нажать Code, выбрать HTTPS, скопировать ссылку на репозиторий, в gitbash зайти в папку, где будет размещен репозиторий),
git clone https://github.com/tsitlau/XML.git
cd JSON - в терминале перейти в папку JSON, в конце адреса расположения отображается main


 23. Внутри локального XML создать файл “new.xml”.
touch new.xml

 24. Добавить файл под гит.
git add new.xml

 25. Закоммитить файл.
git commit -m "add new.xml"

 26. Отправить файл на внешний GitHub репозиторий.
git push

 27. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
vim new.xml
insert
<?xml version="1.0" encoding="UTF-8"?>
<aboutme>
	<fullName>Tatyana Tsitlau</fullName>
	<age>33</age>
	<pets>1</pets>
	<desiredSalary>900$</desiredSalary>
</aboutme>
Esc
:wq

 28. Отправить изменения на внешний репозиторий.
git add new.xml
git commit -m "modified new.xml"
git push

 29. Создать файл preferences.xml
cat > preferences.xml

 30. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
<?xml version="1.0" encoding="UTF-8"?>
<myPreferences>
	<Movie>The Shawshank Redemption</Movie>
	<TvSeries>The Beauty Inside</TvSeries>
	<Food>pizza</Food>
	<Season>summer</Season>
	<Country>Japan</Country>
</myPreferences>
ctrl+D

 31. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
cat > sklls.xml
<?xml version="1.0" encoding="UTF-8"?>
<sklls>
	<one>Базовая теория (Что такое тестирование, багрепорты, документация, виды, методы, направления тестирования и т.п.) SDLC, STLC</one>
	<two>Что такое клиент-серверная архитектура</two>
	<three>HTTP Методы запросов на сервер</three>
	<four>Коды ответов HTTP сервера</four>
	<five>Структуры HTTP запросов и ответов</five>
	<six>Что такое JSON, XML. Их структура</six>
	<seven>Тестирование API через Postman (JS, автотесты API)</seven>
	<eight>Снятие и чтение логов c внешнего сервера</eight>
	<nine>Снифинг http web трафика через Charles и Fiddler</nine>
	<ten>Dev Tools веб браузеров (Google Chrome, FireFox)</ten>
	<eleven>VPN. (Как работает, зачем нужен, как использовать, варианты инструментов)</eleven>
	<twelve>Мобильное тестирование</twelve>
	<thirteen>Особенность iOS, Android, гайдлайны</thirteen>
	<fourteen>Сборка iOS приложений на XCode</fourteen>
	<fifteen>Сборка Android приложений на Android Studio</fifteen>
	<sixteen>ADB (управление андройд девайсами)</sixteen>
	<seventeen>Настройка прокси и vpn на iOS и Android</seventeen>
	<eighteen>Перехват (сниффинг) мобильного трафика через Charles и Fiddler на iOS и Android</eighteen>
	<nineteen>Командная строка (terminal) Linux (копирование, создание, просмотр, перемещение файлов на серверах без графического интерфейса)</nineteen>
	<twenty>Основы bash скриптинг, автоматизация рутинных задач на сервере</twenty>
	<twentyOne>Доступ к удалённым серверам</twentyOne>
	<twentyTwo>Основы SQL (Create, Delete, Drop, Insert Into, Select, From, Where, Join)</twentyTwo>
	<twentyThree>База данных Postgres (установка, настройка и использование)</twentyThree>
	<twentyFour>Нереляционная база данных Redis (установка, настройка и использование)</twentyFour>
	<twentyFive>Нагрузочное тестирование в Jmeter</twentyFive>
	<twentySix>Методология разработки Scrum</twentySix>
	<twentySeven>Python. (Изучение основ. Создание клиент серверного приложения)</twentySeven>
</sklls>
ctrl+D

 32. Сделать коммит в одну строку.
 33. Отправить сразу 2 файла на внешний репозиторий.
git add preferences.xml sklls.xml ; git commit -m "add 2 files" ; git push

 34. На веб интерфейсе создать файл bug_report.xml.
Войти в репозиторий XML. Нажать кнопку Add file.
Выбрать Create new file. В поле Name your file ввести bug_report.xml

 35. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Нажать кнопку Commit new file

 36. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
Открыть файл bug_report.xml. Выбрать редактирование. Ввести текст
<?xml version="1.0" encoding="UTF-8"?>
<Bug>
	<id>5</id>
	<Title>Top and bottom white dash line not visible for size W:242 H:546</Title>
	<Severity>Major</Severity>
	<Priority>high</Priority>
	<Environment>
		<one>Samsung Galaxy s10e, Android 12</one>
		<two>Samsung Galaxy М52, Android 11 ONE UI</two>
		<three>Samsung Galaxy S8, Android 9.0</three>
		<four>Samsung Galaxy Note 8, Android 9.0</four>
		<five>Samsung Galaxy A20, Android 11</five>
		<six>Samsung Galaxy A32, Android 11</six>
		<seven>Samsung Galaxy A7, Android 10</seven>
 	</Environment>
  	<Precondition>Widget on Home screen 4x5</Precondition>
	<STR> 
		<one>Open app</one>
		<two>Tap the "Add Widget" button</two>
		<three>Tap on the widget, start resizing</three>
	</STR>
	<AR>When resizing the widget W:242 H:546 the white dash lines above and below are not displayed</AR>
	<ER>When the widget is resized, the white dash lines along the outline are displayed</ER>
	<Attachments>https://disk.yandex.ru/i/J8npWOfTCPP6WA</Attachments>
</Bug>

 37. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
Нажать параметр Commit changes

 38. Синхронизировать внешний и локальный репозиторий XML
git pull

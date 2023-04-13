# httpProtocol
По адресу https://raw.githubusercontent.com/netology-code/jd-homeworks/master/http/task1/cats находится список фактов о кошках. Наша задача - сделать запрос к этому ресурсу и отфильтровать факты, за которые никто не проголосовал (поле upvotes).
Программа должна прочитать весь список и вернуть только те факты, у которых поле upvotes не равно null или нулю.

Перед тем как начать откройте url https://raw.githubusercontent.com/netology-code/jd-homeworks/master/http/task1/cats в браузере и посмотрите на данные;

Создайте проект maven и добавьте в pom.xml библиотеку apache httpclient
Создайте метод в который добавьте и настройте класс CloseableHttpClient например с помощью builder
Добавьте объект запроса HttpGet request = new HttpGet("https://raw.githubusercontent.com/netology-code/jd-homeworks/master/http/task1/cats") и вызовите удаленный сервис CloseableHttpResponse response = httpClient.execute(request);

Добавьте в pom.xml библиотеку для работы с json
Создайте класс, в который будем преобразовывать json ответ от сервера. Преобразуйте json в список java объектов. Отфильтруйте список - например, средствами stream api. Выведите результат на экран.

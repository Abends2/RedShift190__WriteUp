
<p align="center"><img src="https://github.com/Abends2/RedShift190__WriteUp/blob/main/assets/note.png" alt="1"></p>


---
#### WARNING!

У информационной системы хранения воспоминаний заканчивается время ожидания. Оставшееся время работы - 48 часов.

---
#### Режим нормального функционирования восстановлен, спасибо!

Именно в 2102 году меня создал Егор Сашев, участник первой миссии по колонизации Марса - RedShift. Я - хранилище его воспоминаний про те времена, когда он готовился к этой миссии. Я создан для того, чтобы потомки узнали его историю. Неважно, где вы сейчас находитесь - на Марсе, Земле или другой планете нашей Солнечной системы или даже галактики, я расскажу вам эту историю если вы докажете, что близки ему духом.

---
#### Отлично!

В сфере информационной безопасности нужно быть многогранным. Продемонстрируйте еще навыки, и я допущу вас к архиву с мемуарами Егора Сашева.

---
#### Доступ к архиву получен, {{username}}

Обратите внимание, что некоторые данные могут быть повреждены.

```
#### Запись 1 ####

Меня зовут Егор Сергеевич Сашев. Другая информация обо мне в рамках этих воспоминаний не имеет значения. Сегодня мне исполнилось 98 лет и я наконец решил рассказать о том, как я попал в первую программу колонизации Марса RedShift. Строго говоря, впервые нога отечественного космонавта ступила на поверхность красной планеты в 2048 году, экипаж Николая Иванова доставил туда первую партию материалов для постройки марсианской базы. Миссия колонизации планировалась в 2051м.

#### Конец записи 1 ####
```

---
#### Флаг получен, продолжаем

```
#### Запись 2 ####

С детства я мечтал о покорении космоса, но судьба распорядилась иначе - я работал в сфере компьютерной безопасности и не мог претендовать на место среди космонавтов, которые в то время уже вовсю бороздили околоземное космическое пространство. Миссия по колонизации всё изменила. Набор космонавтов происходил по всей территории нашей необъятной. Нужны были все - биологи, геодезисты, программисты, архитекторы. Это был мой шанс - программировал я неплохо и был в хорошей физической форме.

#### Конец записи 2 ####
```

---
#### #### Флаг получен, продолжаем

```
#### Запись 3 ####

Хотел рассказать о процессе отбора, о его несправедливости. Но с высоты прожитых лет понимаю, что всё произошло как произошло. Вкратце, я не прошел официальный отбор. По каким причинам - неизвестно, но уже и неважно. Я знал, что если миссия удасться - будут еще отборы на следующие полеты, но я не молодею. Мне было уже 48 лет.

#### Конец записи 3 ####
```

---
#### Флаг получен, продолжаем

```
#### Запись 4 ####

Нужно было что-то делать. Я долго бился в бессилии от происходящего, но в один момент на грани отчаяния в голову мне пришел план. А я ведь когда-то работал в компании, которая занимается производством атомных субсветовых двигателей для наших кораблей типа "Нева". Мой план был таков - попробовать найти точку входа в инфраструктуру организации из пула адресов, который когда-то был доступен из внешней сети - 172.80.50.0/24

#### Конец записи 4 ####
```

---
#### Флаг получен, продолжаем

```
#### Запись 5 ####

Я нашел АРМ с адресом 172.80.50.10 с открытыми портами для FTP и SSH. Авторизация по SSH была по паре log+pass, пользователя и пароль подобрать сходу у меня не получилось. Поэтому я решил на удачу попробовать зайти на FTP под anonymous, и это получилось! Среди файлов, доступных мне я обнаружил ToDo лист, в котором фигурировал некий Kevin - наверное наш заморский гастарабайтер. Так как других вариантов не было, я решил использовать это имя как логин для брута ssh. И да, это получилось с помощью rockyou.

#### Конец записи 5 ####
```

---
#### Флаг получен, продолжаем

```
#### Запись 6 ####

На этой машине был еще один сетевой интерфейс, который смотрел в сеть 192.168.20.0/24. Чтобы просканировать её со своей kali нужно было настроить proxychains.

#### Конец записи 6 ####
```

---
#### Флаг получен, продолжаем

```
#### Запись 7 ####

В процессе сканирования обнаружена БД postgreSQL на компьютере пользователя. Этим пользователем была Изабель Кастильон, ответственная за формирование участников программы колонизации от CyberAtom. Я вспотел, потому что понял - на её компьютере может быть список кандидатов, мне нужно дописать себя в него!

#### Конец записи 7 ####
```

---
#### Флаг получен, продолжаем

```
#### Запись 8 ####

По дефолтным кредам подключиться к БД не получилось, а брутфорс не дал результатов. Нужно было искать другой вектор. Я продолжил сканировать сеть...

#### Конец записи 8 ####
```

---
#### Флаг получен, продолжаем

```
#### Запись 9 ####

По адресу 192.168.)*&&:" я нашел контроллер домена. Но как на него залогиниться? Те креды, что были у меня, не подходили. И тут я вспомнил про ToDo лист, который нашел на FTP. Там была запись о том, что нужно проверить файл обновления для Windows Server. Самого файла там пока не было, поэтому я решил создать его. С помощью msfvenom (￣□￣」)

#### Конец записи 9 ####
```

---
#### Флаг получен, продолжаем

```
#### Запись 10 ####

Я слушал порт... Через несколько часов рыбка попалась на крючок - я получил shell. Понятное дело, мне не составило труда получить учетную запись от компьютера Изабеллы, на котором я добавил своё имя в БД, в которой хранились записи о кандидатах на полёт.

#### Конец записи 10 ####
```

На этом записи от Егора Сашева в архиве заканчиваются, но в процессе регулярного сканирования базы данных я обнаружил новые записи, причем датированные 2123 годом. Хотите взглянуть?

---
#### Флаг получен, продолжаем

```
#### Запись 11 ####

Не знаю что сюда написать... Сформирую записи так же, как и предыдущий оратор. Меня зовут Богдан Данилов. Я расскажу вам всю правду о Егоре Сашеве. Он разрушил жизнь всей нашей семье. Решите еще таск, уже от меня.

#### Конец записи 11 ####
```

---
#### Флаг получен, продолжаем

```
#### Запись 12 ####

В 2050м году моему деду было 30 лет. Он был выпускником лётной академии и уже 7 лет работал в CyberAtom в должности архитектора компьютеризированных аэрокосмических систем. У него как раз родился сын - мой отец. Семья жила в достатке, дед должен был стать нашей семейной легендой - колонизатором Марса. Именно к этому он готовился всю свою сознательную жизнь. Он был лучшим в своем наборе - команды от CyberAtom. Однако в последний момент по неизвестным причинам его имя исчезло из списка, который его начальница должна была передать в главный аппарат управления миссией. На пике энтузиазма это стало фатальным ударом для моего деда. От такого разочарования он так и не смог оправиться - впал в депрессию, начал пить и избивать жену. Бабушка не выдержала такого обращения и попала в психиатрическую клинику, а деда лишили родительских прав. Мой отец попал в детский дом в 11 лет. В дестком доме отец познакомился с девушкой, Анастасией - моей мамой. В 18 лет, после выхода из детдома, они сразу расписались. Через несколько лет родился я. Жизнь нашей семьи была тяжелой, мы жили на отшибе Химки-8 на Луне. Родители много работали на шахте по добыче фосфора. Это рано подкосило их здоровье.

#### Конец записи 12 ####
```

---
#### Флаг получен, продолжаем

```
#### Запись 13 ####

Я видел всё это и понимал, что только у меня есть возможность вытащить семью из этого печального положения. Мне нужно было освоить какую-то перспективную и высокооплачиваемую профессию. В раннем возрасте я начал изучать IT-технологии: программирование, сети, операционные системы. Я поступил на бюджет в ^(*&#$(2434(*&^&%^_$))). Особенно мне нравилось изучать старые информационные системы и архитектуры.

Теперь самое главное. В 2120 году за нашим скромным ужином в нейронете отцу попалась новость о смерти последнего из первой колонизаторской миссии Марса Егора Сашева. Отец тогда сказал мне "А ведь твой дед должен был в 2051м лететь в составе этой миссии на Марс, он даже прошел все отборы, но в последний момент его имя исчезло из списка участников. С этого начались проблемы нашей семьи. Кстати странно, что вместо него полетел именно Егор Сашев. Он не проходил по возрасту и состоянию здоровья."

#### Конец записи 13 ####
```

---
#### Все? это конец??

```
#### Запись 14 ####

Эти слова не выходили у меня из головы, и я решил узнать подробности тех давних событий. Я знал, что официальный архив старого интернета был уничтожен метеоритом, но в долгих поисках информации о Егоре Сашеве я наткнулся на его старый хостинг, который до сих пор функционировал. Там был этот бот.

Прошло уже более 80 лет с Redshift118, как на Марсе появилась первая колония Межпланетной Российской Федерации. Если я сейчас обнародую те данные, что обнаружил в этом архиве мне всё равно никто не поверит. Но мне достаточно того, что ты, {{username}}, дошел до этой последней записи. Значит ты достаточно умён чтобы понять - тогда, в 2050м году Егор Сашев написал своё имя вместо имени моего деда в участники миссии, а не просто добавил.

#### Конец записи 14 ####
```

---
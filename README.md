# Ответы на вопросы

### Раздел № 1: аппаратное обеспечение
1 Что такое UEFI? Какие функции выполняет?
> Аналог BIOS . Начальная загрузка и инициализация устройств

2 Каким образом можно очистить CMOS в BIOS?
> Перемычкой, снять батарейку 

3 Что такое сокет? Какие модификации сокетов вам известны?
> Разъем процессора- 448, 777, 1155  

4 Чем отличается ОЗУ DDR 2 от ОЗУ DDR 3?
> Другой стандарт - разъем, большая частота, большая скорость работы

5 Что такое SO-DIMM?
> ddr small factor

6 Опишите принципы работы технологии Hyper-Threading?
> Програмное увеличение колличества ядер процессора

7 Почему 32-битные приложения не могут использовать более 4ГБ ОЗУ?
> Потому что они не могут обращаться к секторам памяти далее 2 в 32 степени

8 Какие функции выполняет технология ECC в ОЗУ? Какие плюсы и минусы данной технологии?
> Память с коррекцией ошибок (стоит дороже, работает медленнее)

9 Что означает выражение: «сетевой интерфейс работает в полудуплексном режиме»?
> Поочередно - прием, передача

10 Рабочая станция аварийно завершает работу при запуске приложений, активно использующих ЦПУ.  Какие вы предпримите первые действия для диагностики проблемы?
> Перегрев - нужен мониторинг температуры.

### Раздел № 2: дисковая подсистема
1 Какие аппаратные интерфейсы имеют HDD? Какие их основные различия?
> scsi, sata, sas, ide (разная скорость, области применения)

2 Чем отличается аппаратный RAID-контроллер от программного? Какие сильные и слабые стороны каждого из них?
> Аппаратный раелизован на отдельном контроллере (дороже, возможна реализация кеширования в отдельном модуле памяти), программный на уровне ОС (дешевле, менее надежен ?) 

3 Какие уровни RAID вам известны?
> 0,1,10,5,6

4 Имеем 4 шт. HDD объёмом 256 ГБ. Объединяем имеющиеся HDD в RAID1. Какой получаем объём дискового пространства вновь созданного RAID-массива?
> 256 (или 2 по 265 = два массива)

5 Многие RAID-контроллеры оснащены набором функций «Hot Spare» и «Hot Swap». Какое предназначение данных функций?
> Горячая замена жестких дисков

6 Как скажется на работе оборудования выход из строя 1 диска, входящего в массив RAID5?
> Замедление работы системы

7 Что такое NTFS, FAT, ext3, ext4? В каких ОС нашли применения описанные технологии?
> Типы ФС , windows, linux

В чём базовое отличие FAT от NTFS?
> Ограничение размера файла, не поддерживает secutity permissions

9 HDD на базе SSD технологии обладают высокой скоростью записи/чтения. За счёт чего достигается эта скорость?
> Отсутствие механики

10 Какие слабые стороны вам известны у HDD на базе SSD технологии?
> Проблеммное восстановление в случае физ. повреждения , цена - объем ?

### Раздел № 3: организация ЛВС
1 Напишите названия и опишите назначения каждого уровня модели OSI.
> физический(физические параметры, биты, ethernet кадр) - сетевой(маршрутизация)- транспортный(передача данных сетевому exp. TCP, UDP ) - прикладной(приложения, протоколы высокого уровня exp. HTTP, DNS)  - упрощенная модель TCP/IP
 
2 В чем принципиальное отличие сетевого концентратора от сетевого коммутатора?
> концентратор отправляет пакеты на все порты 

3 Что такое VLAN? Для решения каких задач используется данная технология?
> Логическое разделение сети

4 Что такое маршрутизатор? Какие функциональные задачи он выполняет?
> Выполняеи функции соединения, маршрутизации между сетями

5 На каких частотах работает сеть Wi-Fi?
> 2,4 GHz , 5 GHz

6 Какую скорость передачи данных обеспечивает стандарт 802.11g?
> 54 Mbit/sec

7 IP-адрес, маска подсети, шлюз, адрес DNS-сервера? Что означают данные термины и какую роль они выполняют?
> Идентификация устройства в сети, DNS - разрешение имени в адрес

8 Сколько устройств может содержать сеть с маской сети равной 255.255.255.252?
> 2

9 Правильно ли указан IP-адрес 192.168.256.1? Ответ обоснуйте.
> нет, максимальное значение октета 255

10 Сколько времени займёт передача файла объёмом 2 МБ при пропускной скорости канала 200 кбит/сек.?
> ~ 82 sec

### Раздел № 4: сервисы и работа с консолью
1 Что такое RDP? Для каких целей используется?
> Удаленное управление

2 Что такое VPN? Для каких целей используется?
> Соединение сетей , удаленное подсоединение к хосту (туннельный, транспортный режимы exp. ipsec)

3 Какие действия выполняет команда tracert?
> Демонстрация маршрута до хоста

4 Как выполнять команды от имени администратора в среде Linux?
> sudo

5 Как проверить сетевую доступность удаленного хоста через командную строку?
> ping

6 Что такое эхо-запрос?
> тип icmp запроса

7 Что такое PowerShell?
> Коммандная оболочка windows , позволяющая выполнять скрипты на powershell

8 Как отключить удаленный хост на базе ОС Windows 8.1 в локальной сети используя командную строку?
> shutdown

9 Какие действия выполняет команда “rm –i” в командной строке Linux?
> Запрос подтверждения удаления (пофайлово)

10 Как вызвать «Диспетчер задач» в ОС Windows, подключившись к хосту по RDP?
> compmgmt.msc 

### Раздел № 5: тестирование приложений
1 Объясните что такое тестирование ПО?
>  Проверка соответствия имеющихся результатов ожидаемым от ПО

2 Какие вы знаете основные уровни тестирования ПО?
> Модульное, интеграционное, системное, приемочное

3 Какие основные цели тестирования ПО?
> Поиск несоответствий, ошибок в ПО

4 Когда следует начинать тестировать ПО?
> По окончании написания модулей

5 Когда следует заканчивать тестировать ПО?
> После приемки, выхода релиза

6 Что такое баг-трекер? Какие функции он выполняет?
> Сервис. Система отслеживания задач и ошибок

7 В чем отличие автоматизированного тестирования от ручного? Когда лучше применять каждый метод тестирования?
> Автоматическое - набор интеграционных тестов, ручное - командой тестировщиков. Необходимо применять оба метода параллельно 

8 Назовите несколько причин, которые приводят к появлению ошибок в ПО? 
> Человеческий фактор,плохой уровень коммуникации между заказчиком и разработчиком 

9 Что такое отладка приложения?
> Этап разработки ПО на котором выявляются и исправляются ошибки

10 Приносит ли вам удовольствие поиск ошибок в ПО?
> Иногда

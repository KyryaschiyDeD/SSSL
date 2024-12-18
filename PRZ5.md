# Практика 5
## Макаров Михаил Максимович
## ББМО-02-23
Была создана ВМ с ОС Ubuntu <br></p>
Wazuh — это бесплатная платформа с открытым исходным кодом для обнаружения угроз, мониторинга безопасности, реагирования на инциденты и соблюдения нормативных требований.
___
[Начало](#начало)<br></p>
[Настройка Kali](#kali)<br></p>
[Подключаем агента](#подключаем-агента)<br></p>
[Wazuh Agent](#wazuhagent)<br></p>
[Suricata](#suricata)<br></p>
[OpenVas](#openvas)<br></p>
[Yara](#yara)<br></p>
[Результат](#результат)<br></p>
___

### Начало <a name="начало"></a>

|![](images/5/Снимок%20экрана%202024-12-08%20153231.png)|
|:--:|
|*Создано 2 ВМ, клиент и сервер*|

|![](images/5/Снимок%20экрана%202024-12-08%20154555.png)|
|:--:|
|*По логике практики № 3 был развёрнут Wazuh manager*|

|![](images/5/Снимок%20экрана%202024-12-08%20154705.png)|
|:--:|
|*Была также развёрнута ВМ на Kali Linux*|

### Настройка kali <a name="kali"></a>

|![](images/5/Снимок%20экрана%202024-12-08%20155300.png)|
|:--:|
|*Загрузка пакетов для установки дополнений Virtual Box*|

|![](images/5/Снимок%20экрана%202024-12-08%20155351.png)|
|:--:|
|*Установка гостевых дополнений*|

|![](images/5/Снимок%20экрана%202024-12-08%20165945.png)|
|:--:|
|*Переименование машины*|

|![](images/5/Снимок%20экрана%202024-12-08%20170159.png)|
|:--:|
|*Проверка связи с остальными ВМ, в данном случае с сервером*|

### Wazuh агент <a name="wazuhagent"></a>

|![](images/5/Снимок%20экрана%202024-12-08%20170421.png)|
|:--:|
|*Установка Wazuh агента*|

|![](images/5/Снимок%20экрана%202024-12-08%20170704.png)|
|:--:|
|*Настройка и установка Wazuh агента*|

|![](images/5/Снимок%20экрана%202024-12-08%20170716.png)|
|:--:|
|*Включение wazuh агента*|

|![](images/5/Снимок%20экрана%202024-12-08%20170810.png)|
|:--:|
|*Видим 2 активных клиента сервере*|

|![](images/5/Снимок%20экрана%202024-12-08%20173931.png)|
|:--:|
|*Настраиваем wazuh на клиенте на новые логи*|

|![](images/5/Снимок%20экрана%202024-12-08%20174111.png)|
|:--:|
|*Перезапускаем клиента wazuh и делаем неуспешные попытки входа в систему*|

|![](images/5/Снимок%20экрана%202024-12-08%20174217.png)|
|:--:|
|*Видим результат*|

|![](images/5/Снимок%20экрана%202024-12-08%20174224.png)|
|:--:|
|*События за последние 5 минут*|

|![](images/5/Снимок%20экрана%202024-12-08%20174245.png)|
|:--:|
|*Подробности одного события*|

|![](images/5/Снимок%20экрана%202024-12-08%20174324.png)|
|:--:|
|*Всего событий*|

### Suricata <a name="suricata"></a>

|![](images/5/Снимок%20экрана%202024-12-08%20174534.png)|
|:--:|
|*На клиенте разворачиваем suricata*|

|![](images/5/Снимок%20экрана%202024-12-08%20174653.png)|
|:--:|
|*Скачиваем...*|

|![](images/5/Снимок%20экрана%202024-12-08%20174723.png)|
|:--:|
|*Собираем....*|

|![](images/5/Снимок%20экрана%202024-12-08%20174755.png)|
|:--:|
|*Процесс сборки*|

|![](images/5/Снимок%20экрана%202024-12-08%20174829.png)|
|:--:|
|*Почти всё*|

|![](images/5/Снимок%20экрана%202024-12-08%20175624.png)|
|:--:|
|*Смотрим IP*|

|![](images/5/Снимок%20экрана%202024-12-08%20180223.png)|
|:--:|
|*Информация о сурикате*|

|![](images/5/Снимок%20экрана%202024-12-08%20180546.png)|
|:--:|
|*Получаем правила*|

|![](images/5/Снимок%20экрана%202024-12-08%20180729.png)|
|:--:|
|*Указываем файл сурикаты для wazuh*|

|![](images/5/Снимок%20экрана%202024-12-08%20180756.png)|
|:--:|
|*Перезапускаем сурикату и вазух*|

|![](images/5/Снимок%20экрана%202024-12-08%20193538.png)|
|:--:|
|*Список последних действий*|

### Прошлые действия так нормально и не зафункционировали, так что делаем по новой

|![](images/5/Снимок%20экрана%202024-12-08%20193608.png)|
|:--:|
|*Ставим сурикату*|

|![](images/5/Снимок%20экрана%202024-12-08%20193622.png)|
|:--:|
|*Получаем правила и разворачиваем*|

|![](images/5/Снимок%20экрана%202024-12-08%20193635.png)|
|:--:|
|*Настраиваем сурикату*|

|![](images/5/Снимок%20экрана%202024-12-08%20193650.png)|
|:--:|
|*Настраиваем сурикату*|

|![](images/5/Снимок%20экрана%202024-12-08%20193713.png)|
|:--:|
|*Смотрим IP*|

|![](images/5/Снимок%20экрана%202024-12-08%20193737.png)|
|:--:|
|*Настраиваем Wazuh*|

|![](images/5/Снимок%20экрана%202024-12-08%20193805.png)|
|:--:|
|*Пингуем клиента*|

|![](images/5/Снимок%20экрана%202024-12-08%20193900.png)|
|:--:|
|*Дополнительно пингуем с ОС kali*|

|![](images/5/Снимок%20экрана%202024-12-08%20193943.png)|
|:--:|
|*Настраиваем фильтры в wazuh веб-морде*|

|![](images/5/Снимок%20экрана%202024-12-08%20193954.png)|
|:--:|
|*Видим сообщения от сурикаты*|

|![](images/5/Снимок%20экрана%202024-12-08%20194029.png)|
|:--:|
|*Подробности одного сообщения*|

### OpenVas <a name="openvas"></a>

|![](images/5/Снимок%20экрана%202024-12-14%20174501.png)|
|:--:|
|*Дополнительно разворачиваем ВМ под openVas*|

|![](images/5/Снимок%20экрана%202024-12-14%20175230.png)|
|:--:|
|*Обновляем систему и ставим докер*|

|![](images/5/Снимок%20экрана%202024-12-14%20175249.png)|
|:--:|
|*Логинимся*|

|![](images/5/Снимок%20экрана%202024-12-14%20175258.png)|
|:--:|
|*Успешный успех*|

|![](images/5/Снимок%20экрана%202024-12-14%20175320.png)|
|:--:|
|*Получаем OpenVas*|

|![](images/5/Снимок%20экрана%202024-12-14%20175458.png)|
|:--:|
|*После всех манипуляций перезагружаемся*|

|![](images/5/Снимок%20экрана%202024-12-14%20175743.png)|
|:--:|
|*Стартуем докер*|

|![](images/5/Снимок%20экрана%202024-12-14%20180346.png)|
|:--:|
|*Радуемся веб-морде greenbone*|

|![](images/5/Снимок%20экрана%202024-12-14%20180624.png)|
|:--:|
|*Подключаемся к docker образу и получаем правила сканирования*|

|![](images/5/Снимок%20экрана%202024-12-14%20180640.png)|
|:--:|
|*Между делом знакомимся с веб интерфейсом*|

|![](images/5/Снимок%20экрана%202024-12-14%20190800.png)|
|:--:|
|*Продолжаем получать правила*|

|![](images/5/Снимок%20экрана%202024-12-14%20203350.png)|
|:--:|
|*Завершили получение*|

|![](images/5/Снимок%20экрана%202024-12-14%20205839.png)|
|:--:|
|*Синхронизируемся*|

|![](images/5/Снимок%20экрана%202024-12-14%20205852.png)|
|:--:|
|*Полная история действий внутри образа*|

|![](images/5/Снимок%20экрана%202024-12-14%20210012.png)|
|:--:|
|*Идём в задачи, читаем сообщение*|

|![](images/5/Снимок%20экрана%202024-12-14%20230528.png)|
|:--:|
|*С докер образа проверяем "хостовую" для него машину*|

|![](images/5/Снимок%20экрана%202024-12-14%20230614.png)|
|:--:|
|*Ждёмс*|

|![](images/5/Снимок%20экрана%202024-12-14%20230739.png)|
|:--:|
|*Нагрузка на систему во время проверки*|

|![](images/5/Снимок%20экрана%202024-12-14%20231004.png)|
|:--:|
|*Нагрузка на основную систему*|

|![](images/5/Снимок%20экрана%202024-12-14%20232333.png)|
|:--:|
|*Дополнительно просканим ещё клиента на ubuntu*|

|![](images/5/Снимок%20экрана%202024-12-14%20232348.png)|
|:--:|
|*Старт*|

|![](images/5/Снимок%20экрана%202024-12-14%20232435.png)|
|:--:|
|*Процесс идёт*|

|![](images/5/Снимок%20экрана%202024-12-14%20232647.png)|
|:--:|
|*Завершён*|

|![](images/5/Снимок%20экрана%202024-12-14%20232806.png)|
|:--:|
|*Изучаем результаты*|

|![](images/5/Снимок%20экрана%202024-12-14%20232824.png)|
|:--:|
|*Изучаем результаты*|

|![](images/5/Снимок%20экрана%202024-12-14%20233509.png)|
|:--:|
|*Изучаем результаты*|

|![](images/5/Снимок%20экрана%202024-12-14%20233518.png)|
|:--:|
|*Количество правил сканирования*|

### Yara <a name="yara"></a>

|![](images/5/Снимок%20экрана%202024-12-14%20234402.png)|
|:--:|
|**|

|![](images/5/Снимок%20экрана%202024-12-14%20234617.png)|
|:--:|
|*На сервере wazuh добавляем в конфиг*|

|![](images/5/Снимок%20экрана%202024-12-14%20234634.png)|
|:--:|
|*Создаём файл для распознавания сообщений yara*|

|![](images/5/Снимок%20экрана%202024-12-14%20234703.png)|
|:--:|
|*Содержимое файла*|

|![](images/5/Снимок%20экрана%202024-12-14%20234751.png)|
|:--:|
|*Добавляем ещё правила и перезапускаем wazuh сервер*|

|![](images/5/Снимок%20экрана%202024-12-14%20234939.png)|
|:--:|
|*На клиенте получаем штуки для работы с yara*|

|![](images/5/Снимок%20экрана%202024-12-14%20235401.png)|
|:--:|
|*Устанавливаем yara*|

|![](images/5/Снимок%20экрана%202024-12-14%20235723.png)|
|:--:|
|*Успешный успех*|

|![](images/5/Снимок%20экрана%202024-12-14%20235819.png)|
|:--:|
|*Создаём файл для работы yara*|

|![](images/5/Снимок%20экрана%202024-12-14%20235857.png)|
|:--:|
|*Полный список последних действий*|

|![](images/5/Снимок%20экрана%202024-12-14%20235905.png)|
|:--:|
|*Смотрим собственно логи*|

|![](images/5/Снимок%20экрана%202024-12-15%20000039.png)|
|:--:|
|*Создаём пару файлов*|

|![](images/5/Снимок%20экрана%202024-12-15%20001412.png)|
|:--:|
|*Получаем правила*|

|![](images/5/Снимок%20экрана%202024-12-15%20002833.png)|
|:--:|
|*Создадим ешё файл с правилами*|

### После этого были совершены плохие действия, которые привели к уничтожению ВМ клиента Ubuntu, делаем по новой на kali 

|![](images/5/Снимок%20экрана%202024-12-15%20004431.png)|
|:--:|
|*Проверка yara после установки*|

|![](images/5/Снимок%20экрана%202024-12-15%20004546.png)|
|:--:|
|*Скачиваем правила yara*|

|![](images/5/Снимок%20экрана%202024-12-15%20004654.png)|
|:--:|
|*Создаём файл для работы yara*|

|![](images/5/Снимок%20экрана%202024-12-15%20004808.png)|
|:--:|
|*Редактикуем файл конфигурации wazuh-agent, добавляем директорию /root в реальном времени*|

|![](images/5/Снимок%20экрана%202024-12-15%20004943.png)|
|:--:|
|*На сервере прописываем параметры для распознавания событий yara*|

|![](images/5/Снимок%20экрана%202024-12-15%20005024.png)|
|:--:|
|*Конфиг файл wazuh на сервере, добавляем yara*|

|![](images/5/Снимок%20экрана%202024-12-15%20005349.png)|
|:--:|
|*Последние действия на сервере*|

|![](images/5/Снимок%20экрана%202024-12-15%20005430.png)|
|:--:|
|*Получаем плохие файлы на клиенте kali*|

|![](images/5/Снимок%20экрана%202024-12-15%20005204.png)|
|:--:|
|*Применили фильтры и видим события yara*|

__________________________________________________________

## Итог: <a name="результат"></a>
### Был создан стенд
### Развёртут Wazuh и был настроен вывод логов из файла авторизации
### Была настроена Suricata
### Был настроен OpenVas
### Была настроена Yara
## Был подготовлен данный отчёт
__________________________________________________________

# Практика 5
## Выполнил студент группы ББМО-02-23
## Макаров Михаил Максимович
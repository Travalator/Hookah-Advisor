# Hookah-Advisor
Чат-бот в Telegram, помогающий выбрать табак для кальяна.

Участники
---------
- Травников Владислав - 19144
- Сахаров Данил - 19144
- Гарипов Тимур - 19144

Проблема
--------

Иногда, даже опытным любителям кальяна трудно определиться с выбором табака, не говоря уже о начинающих. Люди тратят силы и время на поиск подходящего по настроению, вкусу и предпочтениям табака.  
Основные сценарии использования
-------------------------------
- Пользователь, не имеющий опыта в выборе табака, не знает, какие предложения существуют и какие из них наиболее подходящие и качественные. 
- Пользователь, уже имеющий имеющий опыт в курении кальянов, хочет выбрать новый вкус, но не осведомлен о новинках и их качестве.
- Пользователь хочет следить за своими предпочтениями (что он уже пробовали, понравилось ему или нет, какие характеристи он отметил(крепость, вкус и тд)). 

Основные компоненты системы
---------------------------

- Представление
  - Bot API
  - Модуль взаимодействия с Bot API (Общается с Bot API запросами)
  - Модуль парсинга ответа Телеграма (Преобразует JSON в объект Сообщение, вызывает соответствующие )
  - Модуль формирования ответа пользователю (обратное преобразование, рендеринг сообщений)
- Модель
- База данных
- Модуль взаимодействия с базой данных
- To be continued...


Точки расширения
----------------
- С ро



- Разные виды статистики (в бд хранится дата появления растения и информация о нём, на основе её можно составить список всех растений с их возрастом, график полива на неделю и т.д.). Подключается в модели и приложении.
- Работа с разными базами данных. Подключается в модуле взаимодействия с БД, интерфейс (для модуля)
- Разные виды напоминаний: периодические (например, полив, подкормка и т.д.) и разовые (например, выращивание рассады). Подключается в модели. 

Паттерны
--------
- Одиночка – для работы с БД 
- Строитель – для формирования ответов
- Посредник – для работы приложения
- Наблюдатель  – связь представления и приложения для отправки уведомлений (представление подписывается)

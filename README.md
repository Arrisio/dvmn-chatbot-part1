### Курс "Чат-боты на Python"
https://dvmn.org/modules/chat-bots/lesson/devman-bot/

## Урок 1
Телеграм-бот для отслеживания статуса проверки отправленных на проверку задач образовательного ресурса [dvmn.org](https://dvmn.org/).

### Фунционал:
* Программа опрашивает API сайта [dvmn.org](https://dvmn.org/) в режиме long-polling
* В случае ответа сервера с полезной информацией формируется сообщение для отправки пользователю через Телеграм бота.
* Логи отправляются второму боту.

### Как установить

1. Склонировать репозиторий с кодом
```
git clone https://github.com/Arrisio/dvmn-chatbot-part1.git
cd dvmn-chatbot
````
2. Создайте и активируйте виртуальное окружение
*Python3 должен быть уже установлен.*
*Далее приведены команды для UNIX системы*
```
$ python3 -m venv env
$ source env/bin/activate

```
3. Затем используйте `pip` (или `pip3`, есть конфликт с Python2) для установки зависимостей:
```
$ pip install -r requirements.txt
```
4. Запуск приложения
```
$ python main.py
```

### Переменные окружения
Трубеутся следующие переменые окружения :
- `BOT_TOKEN`=токен вашего бота. [Как получить токен бота](https://tlgrm.ru/docs/bots).
- `DVMN_TOKEN`=токен для работы с API Devman. [DVMN's API](https://dvmn.org/api/docs/).
- `SUBSCRIBER_CHAT_ID`=Ваш чат ID в телеграм. Чтобы его узнать, отправьте сообщение @userinfobot.


### Цель проекта

Код написан в образовательных целях на онлайн-курсе для веб-разработчиков [dvmn.org](https://dvmn.org/).
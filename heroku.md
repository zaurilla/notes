### Общая информация

Heroku - платформа для развертывания веб приложений. Подходит для развертывания бота для telegram

В каталоге обязательно должен быть `__init__.py`, подойдет и пустой

### Pipfile

Pipfile.lock лучше не создавать, т.к. тогда heroku сам подберет правильные версии модулей

Procfile должен иметь одну строку, команду запуска сервера `worker: python server.py`, где **worker** - dynos от heroku

### Переменные среды

Установка переменной среды
> `heroku config:set TOKEN=1234567890qwerty`

Получение переменной среды
> `heroku config:get TOKEN`

Получение всех переменных среды
> `heroku config`

Сброс переменной среды
> `heroku config:unset TOKEN`

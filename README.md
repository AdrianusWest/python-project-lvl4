### Hexlet tests and linter status:
[![Actions Status](https://github.com/AdrianusWest/python-project-lvl4/workflows/hexlet-check/badge.svg)](https://github.com/AdrianusWest/python-project-lvl4/actions)
![Python CI](https://github.com/AdrianusWest/python-project-lvl4/actions/workflows/pyci.yml/badge.svg)](https://github.com/AdrianusWest/python-project-lvl4/actions/workflows/pyci.yml)
[![Maintainability](https://api.codeclimate.com/v1/badges/dd3e13d1e3bbd6c4d178/maintainability)](https://codeclimate.com/github/AdrianusWest/python-project-lvl4/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/dd3e13d1e3bbd6c4d178/test_coverage)](https://codeclimate.com/github/AdrianusWest/python-project-lvl4/test_coverage)


# Диспетчер задач (Task Manager)

Четвертый учебный проект курса Hexlet "Python-разработчик".

## О проекте

- Task Manager - это веб-приложение, которое используется для напоминания о запланированных событиях. 
- Может использоваться несколькими пользователями одновременно.
- Реализованы регистрация и авторизация.
- Задачи имеют метки и статусы.

## Как установить и использовать

### Установить
```
git clone https://github.com/AdrianusWest/python-project-lvl4
cd python-project-lvl4
make install
```

### Переменные окружения

Чтобы приложение работало, необходимо создать файл .env в корне проекта.

Затем откройте этот файл и установите любое значение для SECRET_KEY='anything'.

Если вы хотите включить режим отладки, то установите для параметра DEBUG=Yes

### Запуск приложения на локальном сервере

```
make runserver
```

### База данных

Если будет использоваться использовать PostgreSQL, то потребуется установить для переменной окружения DB_POSTGRES=True

Затем задайте необходимые значения для следующих переменных:

POSTGRES_NAME='имя_базы_данных'

POSTGRES_USER='имя_пользователя_базы_данных'

POSTGRES_PASSWORD='пароль_пользователя'

POSTGRES_HOST='хост'

POSTGRES_PORT='порт'

### Применить миграции

```
make migrate
```

### Логирование

Rollbar используется для протоколирования.

Установите для переменной окружения ACCESS_TOKEN='token_вашего_аккаунта_в_роллбаре'

### Язык

Если вы хотите изменить язык на английский, то в task_manager/settings измените значение LANGUAGE_CODE=en

Если вы хотите добавить другой язык, то воспользуйтесь следующим [руководством](https://djangowaves.com/tutorial/multiple-languages-in-Django).

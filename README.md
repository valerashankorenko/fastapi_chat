# Мини чат на FastAPI

## О проекте
Мини-чат на FastAPI с использованием вебсокетов и асинхронной базы данных SQLite. Приложение содержит две основные модели: модель пользователей и модель сообщений, что позволяет пользователям отправлять и получать сообщения в реальном времени.

## Цель
Создать простое и эффективное веб-приложение для обмена сообщениями в реальном времени, которое поддерживает множество пользователей одновременно.

## Автор проекта:
Валерий Шанкоренко<br/>
Github: 👉 [Valera Shankorenko](https://github.com/valerashankorenko)<br/>
Telegram: 📱 [@valeron007](https://t.me/valeron007)<br/>
E-mail: 📧 valerashankorenko@yandex.by<br/>

## Стек технологий
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi&logoColor=white)
![Uvicorn](https://img.shields.io/badge/Uvicorn-003B2D?style=flat-square&logo=uvicorn&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-3F4B3D?style=flat-square&logo=sqlalchemy&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-0D4D3A?style=flat-square&logo=alembic&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-4B8BBE?style=flat-square&logo=pydantic&logoColor=white)
![Bcrypt](https://img.shields.io/badge/Bcrypt-4B8BBE?style=flat-square&logo=python&logoColor=white)
![Passlib](https://img.shields.io/badge/Passlib-4B8BBE?style=flat-square&logo=python&logoColor=white)
![Python-Jose](https://img.shields.io/badge/Python%20Jose-4B8BBE?style=flat-square&logo=python&logoColor=white)
![Websockets](https://img.shields.io/badge/Websockets-4B8BBE?style=flat-square&logo=python&logoColor=white)
![Aiosqlite](https://img.shields.io/badge/Aiosqlite-4B8BBE?style=flat-square&logo=python&logoColor=white)
![Pydantic Settings](https://img.shields.io/badge/Pydantic%20Settings-4B8BBE?style=flat-square&logo=python&logoColor=white)
![Jinja2](https://img.shields.io/badge/Jinja2-4B8BBE?style=flat-square&logo=python&logoColor=white)

## Как запустить проект локально:
1. Клонировать репозиторий и перейти в его директорию в командной строке:
```shell
git clone git@github.com:valerashankorenko/fastapi_mini_chat.git
```
2. Переход в директорию fastapi_mini_chat
```shell
cd fastapi_mini_chat
```
3. Cоздать и активировать виртуальное окружение:
 - для Linux/MacOS
```shell
python3 -m venv venv
source venv/bin/activate
```
- для Windows
```shell
python -m venv venv
source venv/Scripts/activate
```
4. Обновить пакетный менеджер pip
```shell
python3 -m pip install --upgrade pip
```
5. Установить зависимости из файла requirements.txt:
```shell
pip install -r requirements.txt
```
6. В корневой директории создать файл .env и заполнить своими данными:
```
SECRET_KEY=your_secret_key
ALGORITHM=HS256
```
7. Применение миграций
```shell
alembic upgrade head
```
8. Запуск проекта
```shell
uvicorn app.main:app
```
<img width="1254" height="1254" alt="fastStart" src="https://github.com/user-attachments/assets/b2a8edee-416c-45f1-bd01-fcf1c30be482" />


## RU

# Fast Start

Fast Start — это простая программа для Windows, которая позволяет запускать сразу несколько приложений одним нажатием. Можно создавать разные сценарии запуска для работы, игр, учебы или любых других задач и быстро переключаться между ними.

## Возможности

* Запуск нескольких программ одновременно
* Создание, переименование и удаление сценариев
* Добавление приложений через выбор файла
* Автоматическое сохранение всех изменений
* Простой интерфейс в тёмной теме
* Быстрая и лёгкая работа

## Установка

```bash
git clone https://github.com/krax69/Fast-Start
cd FastStart
pip install psutil
python main.py
```

## Сборка EXE

```bash
pip install pyinstaller
pyinstaller --onefile --windowed --icon=rocket.ico main.py
```

После сборки готовый `.exe` файл появится в папке `dist`.

## Структура проекта

```text
FastStart/
├── main.py
├── scenarios.json
├── rocket.ico
├── README.md
└── requirements.txt
```

## Требования

* Windows 10 / 11
* Python 3.10 или новее
* Tkinter
* psutil

## Лицензия

Проект распространяется по лицензии MIT.

## EN

# Fast Start

Fast Start is a simple Windows launcher that lets you start multiple applications with one click. You can create different launch scenarios for work, gaming, school, or anything else and switch between them whenever you need.

## Features

* Launch several programs at once
* Create, rename and delete scenarios
* Add applications using a file picker
* Automatically save all changes
* Simple dark interface
* Lightweight and fast

## Installation

```bash
git clone https://github.com/krax69/Fast-Start
cd FastStart
pip install psutil
python main.py
```

## Build

```bash
pip install pyinstaller
pyinstaller --onefile --windowed --icon=rocket.ico main.py
```

The compiled executable will be available in the `dist` folder.

## Project Structure

```
FastStart/
├── main.py
├── scenarios.json
├── rocket.ico
├── README.md
└── requirements.txt
```

## Requirements

* Windows 10/11
* Python 3.10+
* Tkinter
* psutil

## License

Released under the MIT License.

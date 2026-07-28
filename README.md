<img width="1254" height="1254" alt="fastStart" src="https://github.com/user-attachments/assets/b2a8edee-416c-45f1-bd01-fcf1c30be482" />


## RU

# Fast Start

Fast Start — это простая программа для Windows, которая позволяет запускать сразу несколько приложений одним нажатием. Можно создавать разные сценарии запуска для работы, игр, учёбы или любых других задач и быстро переключаться между ними.

## Возможности

* Запуск нескольких программ одновременно с задержкой между ними
* Создание, переименование и удаление сценариев
* Добавление программ через выбор файла — поддерживаются `.exe` и ярлыки `.lnk`
* Программы отображаются плитками с настоящими иконками (как в Проводнике)
* Удобный выбор задержки запуска (секунды, стрелками ▲▼)
* Остановка всех программ сценария одним нажатием
* Автоматическое сохранение всех изменений в `scenarios.json`
* Тёмный интерфейс
* Лёгкая и быстрая работа

## Установка

```bash
git clone https://github.com/krax69/Fast-Start
cd FastStart
pip install psutil pywin32 Pillow
python main.py
```

`pywin32` и `Pillow` нужны только для отображения настоящих иконок программ. Без них Fast Start тоже работает — вместо иконок будет использоваться заглушка.

## Сборка EXE

```bash
pip install pyinstaller
pyinstaller --onefile --windowed --name "FastStart" --icon=rocket.ico --hidden-import win32com --hidden-import win32com.client --hidden-import win32timezone main.py
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
* pywin32 и Pillow (опционально, для иконок программ)

## Лицензия

Проект распространяется по лицензии MIT.

## EN

# Fast Start

Fast Start is a simple Windows launcher that lets you start multiple applications with one click. You can create different launch scenarios for work, gaming, school, or anything else and switch between them whenever you need.

## Features

* Launch several programs at once, with a configurable delay between each
* Create, rename and delete scenarios
* Add programs via a file picker — supports both `.exe` files and `.lnk` shortcuts
* Programs are shown as tiles with real icons (just like File Explorer)
* Easy delay selection with a spinner (seconds, ▲▼ arrows)
* Stop every program in a scenario with one click
* Automatically saves all changes to `scenarios.json`
* Dark interface
* Lightweight and fast

## Installation

```bash
git clone https://github.com/krax69/Fast-Start
cd FastStart
pip install psutil pywin32 Pillow
python main.py
```

`pywin32` and `Pillow` are only needed to show real program icons. Fast Start still works without them — a placeholder icon is used instead.

## Build

```bash
pip install pyinstaller
pyinstaller --onefile --windowed --name "FastStart" --icon=rocket.ico --hidden-import win32com --hidden-import win32com.client --hidden-import win32timezone main.py
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
* pywin32 and Pillow (optional, for program icons)

## License

Released under the MIT License.
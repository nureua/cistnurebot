
<h3 align="right"> <a href="README.md"> <img src="https://user-images.githubusercontent.com/87089735/213571353-a9f45178-b7e0-41d0-8148-3241ec9d64b2.png" height="20px"> English </a></h3>

# Telegram-бот CIST

Це Telegram-бот, який надає інформацію про розклад певної групи в Національному університеті радіоелектроніки (НУРЕ). Бот використовує API CIST для отримання інформації про розклад.

## Початок роботи

Щоб користуватися цим ботом, вам потрібно виконати наступні кроки:

1. Створіть нового бота за допомогою [BotFather](https://telegram.me/BotFather) та отримайте токен бота.
2. Увімкніть режим inline для бота, надіславши команду `/setinline` BotFather.
3. Клонуйте цей репозиторій.
4. Встановіть необхідні залежності, запустивши `pip install -r requirements.txt`.
5. Запустіть скрипт `gen_file.py`, щоб згенерувати файл `config.py` в кореневому каталозі проекту. Переконайтеся, що ви вводите токен бота Telegram та назву групи НУРЕ, які вам пропонуються в консолі. Не змінюйте формат введення.
6. Запустіть скрипт `bot.py`, щоб запустити бота.

## Використання

Після запуску бота ви можете взаємодіяти з ним, надсилаючи команди в чат Telegram. Що доступно:

- **Команда ручного оновлення**: Авторизовані користувачі можуть вручну оновити та надіслати поточний розклад на визначений канал за допомогою команди `/update`.
- **Заплановані оновлення**: Щоденні оновлення розкладу надсилаються на вказаний канал Telegram о 7:30 ранку з посинаннями на заняття.
- **Розклад на певну дату**: Користувачі можуть запросити розклад на певну дату за допомогою команди `/schedule [DD.MM]`. Ви можете використовувати її з аргументом дати у форматі DD.MM. Якщо аргумент відсутній, використовується поточний день.
- **Використання в будь-якому чаті**: У режимі inline ви можете використовувати тег бота (@YourBotUsername), щоб вибрати розклад. Наприклад, `@YourBotUsername` покаже розклад на сьогодні, а `@YourBotUsername 13.11` покаже розклад на 13 листопада.

## Співпраця

Якщо ви хочете долучитися до цього проекту, не соромтеся надсилати запит або відкривати питання.

## Ліцензія

Цей проект ліцензований під ліцензією MIT - див. файл [LICENSE](LICENSE) для отримання деталей.

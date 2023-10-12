# Генератор звітів для дисципліни "Програмні та інтсрументальні засоби веб-дизайну"

## Увага
Я не перевірив, чи приймає викладач стиль такого звіту.

## Можливості
- Генерування титулки.
- Вставка вихідного коду.
- Генерація зображення сторінки.

## Вимоги перед використанням
- Python.
- `pip install docx`.
- `pip install python-docx`.
- Chrome або Chromium.

## Використання
```sh
python3 zvit_maker.py group name n path_in path_out
```
Де:
- `group`: строка групи без пробілів та лапок: `КІ-23-1`, `КІ-23-2`.
- `name`: ім'я студента у форматі `'Прізвище ІніціалиБезКрапокТаПробілів'`: `'Попов РО'`.
- `n`: номер практичної роботи.
- `path_in`: шлях до файлів практичної роботи. Ці файли мають бути іменованими за спеціальними правилами, які описані нижче.
- `path_out`: назва файлу, в якому буде збережений звіт практичної роботи.
Приклад: `python3 zvit_maker.py КІ-23-1 'Попов РО' 3 third N3.docx`.

## Правила іменування файлів завдань практичної роботи
Назва файлу має відповідати такому правилу, записаному як регулярний вираз: `[0-9](_[0-9])*\.html`.
Приклади: `1.html`, `2.html`, `1_2.html`, `3_1.html`, і так далі.

## Примітка
Програма може генерувати тимчасові файли. Вона їх не видаляє.
Писалося як потік свідомості, перевірка помилок не гарантується.
# goit-algo2-hw-02

\*\* Оптимізація черги 3D-друку та задача розрізання стрижня

# Опис проекту

## Цей проект містить дві основні задачі:

Оптимізація черги 3D-друку: Програма організовує чергу на друк з урахуванням пріоритетів, обмежень принтера та часу друку.

# 🚀 1. Задача розрізання стрижня: Реалізовано два підходи динамічного програмування для розрізання стрижня з метою отримання максимального прибутку.

# Вимоги до системи

- Для запуску програми необхідно встановити:

- Python 3.11+

- Poetry для керування залежностями

- Встановлення

- Клонуйте репозиторій:

- git clone <repository_url>
- cd <repository_folder>

# Створіть віртуальне середовище та встановіть залежності:

- poetry install

# Активуйте середовище:

- poetry shell

1. Оптимізація черги 3D-друку

Формат вхідних даних

print_jobs = [
{"id": "M1", "volume": 100, "priority": 1, "print_time": 120},
{"id": "M2", "volume": 150, "priority": 1, "print_time": 90},
{"id": "M3", "volume": 120, "priority": 1, "print_time": 150},
]

'printer_constraints = {"max_volume": 300, "max_items": 2}'

Формат вихідних даних

{
"print_order": ["M1", "M2", "M3"],
"total_time": 360
}

- Запуск тестів для 3D-друку

- python optimize_printing.py

# 🚀 2. Задача розрізання стрижня

Формат вхідних даних

length = 5
prices = [2, 5, 7, 8, 10]

- Формат вихідних даних

'{
"max_profit": 12,
"cuts": [2, 2, 1],
"number_of_cuts": 2
}'

- Запуск тестів для розрізання стрижня

- python rod_cutting_memo.py

# Реалізація

# Оптимізація черги 3D-друку

- Програма:

- Сортує завдання за пріоритетами (від 1 до 3) та за часом друку.

- Групує моделі у партії для друку відповідно до обмежень принтера.

- Визначає загальний час друку.

- Оптимальне розрізання стрижня

- Рекурсія з мемоізацією (rod_cutting_memo): використовує збереження результатів підзадач.

- Табуляція (rod_cutting_table): використовує ітеративний підхід із динамічним масивом.

- Автор

Eduard

Ліцензія

Цей проєкт поширюється за ліцензією MIT.

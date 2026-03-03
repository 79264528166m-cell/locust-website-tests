# Нагрузочное тестирование на Locust

Проект для нагрузочного тестирования веб-сайтов с использованием Python и Locust.

## О проекте
Я написала этот проект, чтобы показать навыки нагрузочного тестирования. Здесь есть генерация тестовых данных, разные сценарии поведения пользователей и анализ результатов.

## Технологии
- Python
- Locust
- Faker
- CSV
- Git/GitHub

## Как запустить

### 1. Скачать проект
```bash
git clone https://github.com/ТВОЙ-ЛОГИН/locust-website-tests.git
cd locust-website-tests
2. Настроить окружение
# Создать виртуальное окружение
python -m venv venv

# Активировать (Windows)
venv\Scripts\activate

# Активировать (Mac/Linux)
# source venv/bin/activate
3. Установить зависимости
pip install -r requirements.txt
4. Сгенерировать тестовые данные
python utils/data_generator.py
5. Запустить тест
locust -f locustfile.py
Открой браузер → http://localhost:8089

Введи:

Users: 10

Spawn rate: 2

Host: https://jsonplaceholder.typicode.com

Нажми "Start swarming"

Структура проекта
locust-website-tests/
├── data/              # CSV файлы с тестовыми данными
├── reports/           # Отчеты о тестировании
├── utils/             # Скрипты для генерации данных
├── locustfile.py      # Сценарии тестирования
├── requirements.txt   # Зависимости
└── README.md          # Описание проекта
Сценарии
Главная страница (часто)

Поиск товаров (часто)

Категории (средне)

Карточка товара (средне)

Корзина (редко)

Авторизация (редко)

Результаты
В отчете смотри:

Fails = 0 (нет ошибок)

95% < 500 ms (быстрый ответ)

RPS стабилен

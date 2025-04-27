# AutoParts Store

Це веб-платформа для продажу автозапчастин, де користувачі можуть переглядати продукти, здійснювати замовлення, реєструватися та входити в систему для управління своїми даними.

## Стек технологій:
- **Frontend**: React, Redux, React Router, SCSS
- **Backend**: FastAPI, Pydantic, Tortoise ORM
- **База даних**: SQLite (можна змінити на MySQL або MongoDB)
- **Контейнеризація**: Docker, Docker Compose
- **Аутентифікація**: JWT
- **Розгортання**: Розгортання в хмарному середовищі (наприклад, Heroku, AWS)

## Запуск проекту

1. **Клонувати репозиторій:**
   ```bash
   git clone https://github.com/username/AutoPartsStore.git
   cd AutoPartsStore
   ```
2. **Налаштування бекенду:**

1. Створіть віртуальне середовище для Python:

```
python3 -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```
2. Встановіть залежності:
```
pip install -r backend/requirements.txt
```
3. Запустіть сервер:

```
uvicorn app.main:app --reload
```
3. **Налаштування фронтенду:**

1. Перейдіть до папки фронтенду:

```
cd frontend
```
2. Встановіть залежності:

```
npm install
```
3. Запустіть сервер:
```
npm start
```
4. **Налаштування Docker (опційно):**

1. Створіть Docker контейнер для бекенду та фронтенду:
```
docker-compose up --build
```
## Документація API

Вся документація API доступна за адресою:

```
http://localhost:8000/docs
```
**Структура API:**

POST /api/v1/users/ – створення користувача.

GET /api/v1/users/{user_id} – отримання користувача.

POST /api/v1/login – аутентифікація користувача.

POST /api/v1/orders/ – створення замовлення.

GET /api/v1/orders/ – отримання всіх замовлень.

GET /api/v1/orders/{order_id} – отримання замовлення за ID.

## Тестування

1. Для тестування бекенду використовуйте:
```
pytest
```
2. Для тестування фронтенду використовуйте:
```
npm test
```
## Розгортання

1. Docker: Проект можна розгорнути в будь-якому середовищі, що підтримує Docker. Для цього використовуйте docker-compose для запуску контейнерів.

2. Heroku / AWS: Для розгортання на хмарних платформах (наприклад, AWS, Heroku) необхідно налаштувати CI/CD pipeline.

## Ліцензія
Цей проект ліцензується за умовами MIT License.

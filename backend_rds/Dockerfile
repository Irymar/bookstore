# 1. Базовий образ Python
FROM python:3.11-slim

# 2. Робоча директорія всередині контейнера
WORKDIR /app

# 3. Копіюємо файли у контейнер
COPY . .

# 4. Встановлюємо залежності з requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# 5. Відкриваємо порт
EXPOSE 8000

# 6. Команда запуску Django-серверу
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

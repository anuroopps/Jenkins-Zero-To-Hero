FROM python:3.9-slim

WORKDIR /app

# Install Django
RUN pip install django==3.2

# Copy app code
COPY . .

# Optional: Run migrations in CMD to ensure DB is ready at runtime
EXPOSE 8000

CMD ["sh", "-c", "python manage.py migrate && python manage.py runserver 0.0.0.0:8000"]



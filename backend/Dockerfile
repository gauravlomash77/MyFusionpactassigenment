# Python image
FROM python:3.11-slim

# Working directory
WORKDIR /app

# Backend app files
COPY ./app /app/app
COPY ./requirements.txt /app/

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Port
EXPOSE 8000

# Run FastAPI
CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]

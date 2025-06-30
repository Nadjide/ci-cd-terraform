FROM python:3.9
WORKDIR /app
RUN pip install mysql-connector-python fastapi uvicorn
COPY . .
CMD ["uvicorn", "main:app", "--proxy-headers", "--host", "0.0.0.0", "--port", "8000"]
EXPOSE 8000
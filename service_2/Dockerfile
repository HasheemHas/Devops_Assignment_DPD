FROM python:3.9-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
RUN apt-get update && apt-get install -y curl 
COPY . .
EXPOSE 8002
CMD ["python", "app.py"]


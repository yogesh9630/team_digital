FROM python:3.9-slim

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /app

COPY . /app/

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

#docker build -t myproject .
#docker run -p 8000:8000 myproject
#kubectl apply -f deployment.yaml
#kubectl apply -f service.yaml


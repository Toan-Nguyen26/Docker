# docker run -v "$(pwd):/app" -w /app python:3.9 bash -c "pip install django & python manage.py runserver 0.0.0.0:8000 ."   

FROM python:3.9
WORKDIR /app

COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .

CMD [ "python", "manage.py", "runserver", "0.0.0.0:8000" ]
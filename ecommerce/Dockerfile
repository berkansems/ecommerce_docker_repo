FROM python:3.6.8-jessie

COPY requirements.txt /

RUN pip install -r requirements.txt

RUN mkdir app

COPY . ./app

WORKDIR /app

EXPOSE 8000/tcp

CMD [ "python", "./manage.py", "runserver", "0.0.0.0:8000" ]
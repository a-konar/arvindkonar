FROM python:3.9-slim-buster

WORKDIR /app

COPY ./app/requirements.txt requirements.txt
RUN python3 -m pip install -r requirements.txt

COPY ./app/app.py .

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]
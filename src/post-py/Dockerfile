FROM python:3.6.0-alpine

RUN apk update && apk add python3-dev gcc libc-dev
WORKDIR /app
ADD . /app
ENV POST_DATABASE_HOST post_db
ENV POST_DATABASE posts

#RUN pip install --upgrade pip

RUN pip install --requirement /app/requirements.txt


CMD ["python3", "post_app.py"]

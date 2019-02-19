FROM alpine:3.9

MAINTAINER bbloks

RUN apk add --update \
    python3 \
    python-dev \
    py-pip \
    build-base \
  && pip3 install virtualenv \
  && pip install --upgrade pip \
  && rm -rf /var/cache/apk/*

WORKDIR /app
COPY ./app /app

RUN virtualenv /env && /env/bin/pip3 install -r /app/requirements.txt

EXPOSE 5000

CMD ["/env/bin/python", "main.py"]
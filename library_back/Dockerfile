FROM python:3.10-alpine

RUN apk update && apk add postgresql-dev gcc python3-dev musl-dev

RUN mkdir -p /library_back

WORKDIR /library_back

COPY . .

RUN pip install -r requirements.txt

EXPOSE 8000

ENTRYPOINT [ "sh", "entrypoint.sh" ]
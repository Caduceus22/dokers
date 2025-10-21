FROM python:alpine

COPY requirements.txt /temp/

WORKDIR /service

EXPOSE 8000

RUN pip install -r /temp/requirements.txt

COPY . .

RUN adduser --disabled-password service-user

USER service-user


# CMD [ "npm", "run", "dev" ]

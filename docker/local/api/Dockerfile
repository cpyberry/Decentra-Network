FROM python:3.8-alpine

LABEL org.opencontainers.image.source https://github.com/Decentra-Network/Decentra-Network

RUN mkdir /app

RUN apk update

WORKDIR /app/

COPY Decentra-Network Decentra-Network

RUN pip install --no-cache-dir -r Decentra-Network/requirements/api.txt

CMD [ "python3", "Decentra-Network/decentra_network/api/main.py"]

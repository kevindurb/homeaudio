FROM python:alpine

RUN apk add git

WORKDIR /root/
RUN git clone https://github.com/xkonni/snapcastr
WORKDIR /root/snapcastr
RUN pip3 install .

EXPOSE 5000

CMD snapcastrd --bind 0.0.0.0 --host snapcast

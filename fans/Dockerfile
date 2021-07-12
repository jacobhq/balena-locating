FROM ubuntu

RUN apt-get -y update
RUN apt-get -y install cron

ADD crontab /etc/cron.d/fan-cron

RUN chmod 0644 /etc/cron.d/fan-cron

RUN i2cset -y 1 0x01a 0xfe

CMD cron

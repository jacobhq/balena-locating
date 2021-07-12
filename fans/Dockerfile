FROM ubuntu

RUN apt-get -y install cron

ADD crontab /etc/cron.d/fan-cron

RUN chmod 0644 /etc/cron.d/fan-cron

CMD cron

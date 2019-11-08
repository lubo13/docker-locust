FROM ubuntu:18.04

RUN apt-get update && apt-get install -y wget python3-software-properties python-pip git-core supervisor

COPY ./supervisor.conf /etc/supervisor/supervisord.conf

RUN pip install locustio

RUN mkdir -p /var/www/locust

RUN git clone https://Lubo13@bitbucket.org/Lubo13/locust.git /var/www/locust

ENTRYPOINT ["supervisord", "-c", "/etc/supervisor/supervisord.conf"]

RUN echo "Touch in browser http://localhost:8089"
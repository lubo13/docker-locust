FROM ubuntu:18.04

RUN apt-get update && apt-get install -y wget python3-software-properties python-pip git-core

RUN pip install locustio

RUN mkdir -p /var/www/locust

RUN git clone https://Lubo13@bitbucket.org/Lubo13/locust.git /var/www/locust

ENTRYPOINT  ["ln", "-sf", "/var/www/links/links.py", "/var/www/locust/links/"]
ENTRYPOINT  ["locust", "-f", "/var/www/locust/locust_file.py", "-H"]

RUN echo "Touch in browser http://localhost:8089"
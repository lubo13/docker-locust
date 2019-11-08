# README #

This README would normally document whatever steps are necessary to get your application up and running.

### What is this repository for? ###

* Build docker image with Phyton - Locust application for stress test
* >  Locust application repo -> https://bitbucket.org/Lubo13/locust

### How do I get set up? ###

* $ sudo apt-get install docker.io
* $ sudo apt-get install docker-compose
* $ git clone git@bitbucket.org:Lubo13/docker-locust.git
* $ cd docker-locust
* $ sudo service docker start
* $ sudo docker-compose build
* Edit urls in ./links.links.py with your urls for test
* Edit WEBSITE_DOMAIN in .env with domain for that you want to make stress test
* $ sudo docker-compose up -d
* Type in browser -> http://localhost:8089
* $ sudo docker-compose down
* $ sudo service docker stop

### Who do I talk to? ###

* Bitbucket Repository -> https://bitbucket.org/Lubo13/docker-locust
* Email -> grozdanov.lubo@gmail.com

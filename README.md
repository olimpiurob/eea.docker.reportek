## Docker orchestration for Data Repositories portals

Docker orchestration for Data Repositories portals


### Installation

1. Install [Docker](https://www.docker.com/).

2. Install [Docker Compose](https://docs.docker.com/compose/).


### Usage for CDR staging

    $ git clone https://github.com/olimpiurob/eea.docker.reportek.git
    $ cd eea.docker.reportek
    $ docker-compose -f docker-compose-staging.yml up -d
    $ docker-compose -f docker-compose-staging.yml logs


### Upgrade CDR staging

    $ sudo docker-compose -f docker-compose-staging.yml stop
    $ sudo docker-compose -f docker-compose-staging.yml rm -v
    $ sudo docker-compose -f docker-compose-staging.yml pull
    $ sudo docker-compose -f docker-compose-staging.yml up -d
    $ sudo docker-compose -f docker-compose-staging.yml logs

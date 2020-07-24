# Code analysis tools packed in one compose file

As of writing, only SonarQube is available, but more will be added in the future.

### Installation
```sh
$ cp .envsample .env
$ docker-compose build --no-cache
```

###### Note: If you make any changes to the environment variables, make sure to build the container again by running the following commands:
#
```
$ docker-compose build --no-cache
```

### Usage

```sh
$ docker-compose up -d
```

Note: If you wish to persist database data in-between runs, make sure that you run `docker-compose stop` instead of `docker-compose down`

###### References:
- https://hub.docker.com/_/sonarqube/
- https://docs.sonarqube.org/latest/setup/get-started-2-minutes/
- https://docs.sonarqube.org/latest/setup/environment-variables/

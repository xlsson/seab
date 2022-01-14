# Svenska Elsparkcyklar AB
A student project for the course Pattern at Blekinge Institute of Technology, BTH, autumn 2021.

This repo contains a docker-compose file that runs docker images. Together, the subsystems make up a system for a fictitious e-scooter rental company.

## Instructions

Run the docker-compose file in a folder containing the following environment files (which need to be obtained separately):

```
.env-bike // For the bike applications
.env-server // For the server
.env-customer-app // For the customer app
.env-customer-web // For the customer web interface
```

The server is connected to a cloud-based database, deployed at MongoDB Atlas.

### Commands

The subsystems can be started as docker containers running in the background, using the below commands. The server service is linked/set as depend_on for all other services, meaning that it is started automatically before another service starts.

```
Command:                            Starts:                  At:  
docker-compose up -d server         Server                   localhost:1337
docker-compose up -d admin          Admin interface          localhost:3000
docker-compose up -d customer-app   Customer app             localhost:3001
docker-compose up -d customer-web   Customer web interface   localhost:3001
docker-compose run bike             Bike program CLI         Command line
docker-compose run sim              Simulation CLI           Command line
```

## Subsystems: repos and docker images

Each subsystem uses CI services such as Github Actions / Travis / Scrutinizer for code quality measurements, and the below repos contain badges with links to each service.

### Server
GitHub repo: [https://github.com/wadholm/pattern-backend](https://github.com/wadholm/pattern-backend)

Docker image: [https://github.com/wadholm/pattern-backend/](https://github.com/wadholm/pattern-backend/)

### Bike applications
GitHub repo: [https://github.com/freddyph/pattern-bikeprogram](https://github.com/freddyph/pattern-bikeprogram)

Docker image bike program: [https://hub.docker.com/r/anau17/bikeprogram](https://hub.docker.com/r/anau17/bikeprogram)

Docker image simulation: [https://hub.docker.com/r/anau17/simulering](https://hub.docker.com/r/anau17/simulering)

### Customer app
GitHub repo: [https://github.com/richardstg/bike-customer-app](https://github.com/richardstg/bike-customer-app)

Docker image: [https://hub.docker.com/r/rist19/pattern-customerwebbinterface](https://hub.docker.com/r/rist19/pattern-customerwebbinterface)

### Customer web interface
GitHub repo: [https://github.com/richardstg/bike-customer-client](https://github.com/richardstg/bike-customer-client)

Docker image: [https://hub.docker.com/r/rist19/pattern-customerapp](https://hub.docker.com/r/rist19/pattern-customerapp)

### Administrative web interface
GitHub repo: [https://github.com/xlsson/pattern-admin](https://github.com/xlsson/pattern-admin)

Docker image: [https://hub.docker.com/repository/docker/xlsson/pattern-admin](https://hub.docker.com/repository/docker/xlsson/pattern-admin)

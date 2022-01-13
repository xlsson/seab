# Svenska Elsparkcyklar AB
A student project for the course Pattern at Blekinge Institute of Technology, BTH, autumn 2021.

This repo contains a docker-compose file, that runs docker images. Together, they make up a system for a fictitious e-scooter rental company.

## Instructions

Run the docker-compose file in a folder containing the following environment files (which should have been made available to you):

```
.env-bike // For the bike applications
.env-server // For the server
.env-customer-app // For the customer app
.env-customer-web // For the customer web interface
```

The server is connected to a cloud-based database, deployed at MongoDB Atlas.

### Commands



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

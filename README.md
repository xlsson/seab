# seab. - Svenska Elsparkcyklar AB
A student project for the course Pattern at Blekinge Institute of Technology, BTH

This repo contains a docker-compose file, that runs docker images making up a system for "seab.", a fictitious e-scooter rental company.

## Instructions

For the docker containers to work, you will need to run the docker-compose file in a folder containing environment files for the server, bike app, customer app and customer web interfaces. If you are authorized to run the system, these environment files should have been made available to you.

### Commands



## Subsystems: repos and docker images

### Server
GitHub repo: [https://github.com/wadholm/pattern-backend](https://github.com/wadholm/pattern-backend)
Docker image: [https://github.com/wadholm/pattern-backend/](https://github.com/wadholm/pattern-backend/)

### Bike application with simulation
GitHub repo: [https://github.com/freddyph/pattern-bikeprogram](https://github.com/freddyph/pattern-bikeprogram)
Docker image bike app: [https://hub.docker.com/r/anau17/bikeprogram](https://hub.docker.com/r/anau17/bikeprogram)
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

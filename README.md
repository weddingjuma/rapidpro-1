[![Build Status](https://travis-ci.org/eHealthAfrica/rapidpro.svg?branch=master)](https://travis-ci.org/eHealthAfrica/rapidpro.svg)

# RapidPro  

RapidPro is a hosted service for visually building interactive messaging applications.
To learn more, please visit the project site at http://rapidpro.github.io/rapidpro.

### Get Involved

To run RapidPro for development, follow the Quick Start guide at http://rapidpro.github.io/rapidpro/docs/development.

### License

In late 2014, Nyaruka partnered with UNICEF to expand on the capabilities of TextIt and release the source code as RapidPro under the Affero GPL (AGPL) license.

In brief, the Affero license states you can use the RapidPro source for any project free of charge, but that any changes you make to the source code must be available to others. Note that unlike the GPL, the AGPL requires these changes to be made public even if you do not redistribute them. If you host a version of RapidPro, you must make the same source you are hosting available for others.

RapidPro has dual copyright holders of UNICEF and Nyaruka.

## Running with docker

Install Requirements:

- Docker
- Docker Compose

Run 

```sh
docker-compose up -d db
docker-compose up -d redis
docker-compose build rapidpro
docker-compose run rapidpro entrypoint.sh setupdb
docker-compose up rapidpro
```

Then visit localhost:5000 (linux) or run

```sh
docker-machine ip default
```
 
on OS X to get the docker machine ip and visit <IP>:5000 in your browser.

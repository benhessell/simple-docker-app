### Simple-docker-app

## Introductions
This project allows a user to input a goal and remove a goal

This project has three parts, backend, frontend, and a mongo database, which is downloaded as an image from docker hub.
There is a docker-compose at the root level, it contains the code to start up a mongo and backend container. 
They talk to each other over a network created by docker-compose
Frontend is not put into a container. In prod-script, I tried to do a script including front-end but it did not work

## Running
To Run BE and mongodb: docker-compose up in dev-script dir
To run mongodb and BE and rebuild images (need to do if change BE code): docker-compose up --build
To run mongodb and BE in detached mode (i.e. no logs): docker-compose up -d

To run frontend: yarn && yarn start
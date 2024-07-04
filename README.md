# Dockerize_express_app

## Implemented following:
https://semaphoreci.com/community/tutorials/dockerizing-a-node-js-web-application

## Running app:
### Running server
```bash
docker build -t <name-of-image> . 
```
```bash
docker compose run <name-of-image> npm start/test/run pm2
```
### Running db ?
``` bash
docker compose up -d
```
### Checking for active container:
```bash
docker ps
```

### Stopping active containers:
```bash
docker compose down
```

## Example of api calls:
### PUT:
```bash
curl -w "\n" \
       -X PUT \
       -d "firstName=Bobbie&lastName=Draper" \
       localhost:3000/persons
```
### GET:
```bash
curl -w "\n" localhost:3000/persons/all
```

## Note:
### Have dockerdesktop running

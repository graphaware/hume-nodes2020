# Nodes 2020 - NLP with GraphAware Hume

This repository contains a trial version of Hume for the Nodes 2020 event. Participants will receive credentials through their registration that they have to use
during the instructions described below.

## Requirements

- A laptop or a server with 5-6GB of memory.
- Docker and Docker Compose installed

## Installation

The following procedure will install the necessary containers for running Hume : 

- Neo4j 4.1.2
- Hume
- Hume Entity Extraction Service
- Hume Keyword Extraction Service

### Login to the GraphAware Docker registry

```bash
docker login docker.graphaware.com
```

and provide the credentials that have been given to you during the registration.

### Pull the containers

```
docker-compose pull
```

### Start Hume

```
docker-compose up -d
```

it can take some minutes to start depending on your machine.

### Inspect logs

If something is not working as expected, inspect the logs : 

```
docker-compose logs -f
```
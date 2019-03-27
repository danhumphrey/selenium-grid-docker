# selenium-grid-docker

Start grid with 1 chrome and firefox node `docker-compose up`

## Scaling 
The nodes can be scaled by starting multiple containers:

`docker-compose up --scale chrome=4 --scale firefox=4`

1 node per container is considered best practice but can be increased by passing in environment variables:
 
`docker-compose up -e NODE_MAX_INSTANCES=4 -e NODE_MAX_SESSION=4`
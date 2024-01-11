# How to use docker-compose for VFK Research MSB

## Files

* __docker-compose.yml:__ Configuration of all available core services
* __.env:__ Compose ENVIRONMENT VARIABLES__ to define MSB~_VERSION and REGISTRY
* __env.list:__ Available __Container ENVIRONMENT VARIABLES__
* * __docker-compose.xyz.yml:__ Configuration of additional services like basyx, ...

## Docker Compose UP

Available core components:

- mysql
- rabbitmq
- vfk-service-discovery
- vfk-msb-gui
- vfk-msb-message-processing
- vfk-msb-connected-service-management
- vfk-msb-interface-websocket
- vfk-msb-interface-rest
- vfk-msb-interface-rest-basyx

## VFK Research MSB Sample Commands

### Configuration

It is necessary to adjust the environment variables marked with <set-username> and <set-secure-password> in env.list file.

### Core components including websocket and rest interface:
````bash
docker-compose up -d \
mysql \
rabbitmq \
vfk-service-discovery \
vfk-msb-gui \
vfk-msb-message-processing \
vfk-msb-connected-service-management \
vfk-msb-interface-websocket \
vfk-msb-interface-rest
````

## VFK MSB Basyx Sample Commands

````bash
docker-compose -f docker-compose.yml -f docker-compose.basyx.yml up -d \
mysql \
rabbitmq \
vfk-service-discovery \
vfk-msb-gui \
vfk-msb-message-processing \
vfk-msb-connected-service-management \
vfk-msb-interface-rest-basyx \
vfk-msb-interface-rest-basyx-mongodb \
basyx-registry-test
````

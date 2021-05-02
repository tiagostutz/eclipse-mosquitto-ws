# Eclipse Mosquitto with Websocket enabled

A ready to use Mosquitto MQTT broker Docker image with WebSocket enabled

## Getting Started

Just bring up the following docker-compose.yml:

```yaml
version: "3.7"

services:

  mqtt:
    image: tiagostutz/eclipse-mosquitto-ws:2.0.10
    restart: always
    network_mode: bridge
    ports:
      - 1883:1883
      - 9001:9001
```

You are ready to connect at TCP on `1883` and at HTTP/Websocket at `9001`
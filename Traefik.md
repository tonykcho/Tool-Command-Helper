# This is an Traefik reverse proxy guide.

In local environment, Traefik require host name to work with. Please add some local hostname to your local DNS.

## Adding local hostname to your own machine.

Modify /etc/hosts file.

127.0.0.1   traefik.localhost
127.0.0.1   traefik.grafana.localhost
127.0.0.1   traefik.prometheus.localhost
127.0.0.1   traefik.jaeger.localhost

## Traefik by default support for Docker. No extra configuration to use it.

In docker compose file. We are required to add labels to the services

```
labels:
- "traefik.enable=true"
- "traefik.http.routers.traefik.rule=Host(`traefik.localhost`)"
- "traefik.http.services.traefik.loadbalancer.server.port=8080"
```

traefik.http.routers.{service_name}.rule=Host(``);
Specify your hostname (DNS).

traefik.http.services.{service_name}.loadbalancer.server.port={port}
Specify which port of the service to reverse proxy. By default, it used the smallest port.
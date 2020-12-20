# rca-docker
experiments with docker container for frontend development

## usage
Run containers

```bash
docker-compose -f docker-compose.yml up --build -d
```

It will create 2 containers. First - `react-create-app` builded with alpine/node14 with default port :3000 in local docker network. 
Second - `nginx` at :9000 host port. 

To watch app, open url:

```
localhost:9000
```

## stats

| container | mem |
| ---       | --- |
| frontend (alpine linux + node14) min (run)   | 200 MB |
| frontend (alpine linux + node14) max (build) | 400 MB |
| nginx | 2 MB |
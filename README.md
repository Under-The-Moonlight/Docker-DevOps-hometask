# Docker-DevOps-hometask

##CLI commands

**Building docker image**

``
docker build -t node-kpi .
``

**Run docker container with limits for cpu and memory and available on port 80**

```
docker run -d --rm --memory=50m --cpus="1.0" --name kpi -p 80:8080 node-kpi
```


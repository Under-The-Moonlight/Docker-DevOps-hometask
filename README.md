# Docker-DevOps-hometask

## CLI commands

**Building docker image**

``
docker build -t node-kpi .
``

**Run docker container with limits for cpu and memory and available on port 80**

```
docker run -d --rm --memory=50m --cpus="1.0" --name kpi -p 80:8080 node-kpi
```

**Push docker image to docker hub**

Firstly, we have to build new image that we will push to docker hub. Instead of 'shchupalco' use your own login

```
docker build -t shchupalco/node-kpi
```

After that we're ready to push it to our repo

```
docker login

docker push shchupalco/node-kpi
```

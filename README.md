# Chore Master

```sh
git submodule update --init --recursive
```

## Deployment

```sh
sudo docker compose -f ./deployments/docker-compose.production.yml up -d --build
sudo docker compose -f ./deployments/docker-compose.production.yml down
```
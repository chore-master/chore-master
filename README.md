# Chore Master

```sh
git submodule update --init --recursive
```

## Deployment

```sh
sudo docker compose -f ./deployments/docker-compose.production.yml -p chore_master_production up -d --build
sudo docker compose -f ./deployments/docker-compose.production.yml -p chore_master_production down
```
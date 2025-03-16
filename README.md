# Chore Master

Chore Master 是一套著重於個人需求的助理，透過模組化的解決方案，將日常瑣事變得更有效率。

# 本地使用

使用 git submodule 下載前端 monorepo 及後端 monorepo 原始碼，預設使用 sqlite 做為資料庫，可依個人喜好調整。

```sh
git submodule update --init --recursive
sudo docker compose -f ./deployments/docker-compose.production.yml -p chore_master_production up -d --build
sudo docker compose -f ./deployments/docker-compose.production.yml -p chore_master_production down
```

# 開發

請分別參閱子專案的 README 進行開發
- [Chore Master Python](https://github.com/chore-master/chore-master-python/blob/main/apps/chore_master_api/README.md)
- [Chore Master Web](https://github.com/chore-master/chore-master-web/tree/main/packages/end-user-app)
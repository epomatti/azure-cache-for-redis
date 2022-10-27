# Azure Cache for Redis

Simple Azure Cache for Redis.

```sh
cd infra

terraform init
terraform apply -auto-approve
```



List the key:

```sh
az redis list-keys -n "redis-caching" -g "rg-caching"
```

Create the `.env`:

```sh
REDIS_CACHE_HOSTNAME="redis-caching.redis.cache.windows.net"
REDIS_CACHE_KEY=""
```

Run the app:

```sh
npm i
npm run start
```

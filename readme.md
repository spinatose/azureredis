### Bash
- Create resource group
`az group create --name az204-redis-rg --location <myLocation>`

- Create Azure Redis Cache
```
redisName=az204redis$RANDOM
az redis create --location <myLocation> \
    --resource-group az204-redis-rg \
    --name $redisName \
    --sku Basic --vm-size c0
```

### Azure Portal
- Get connection string from redis cache just created


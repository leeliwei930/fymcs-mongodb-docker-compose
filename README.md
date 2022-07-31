### MongoDB Docker Compose Configuration Setup


#### Instruction

#### Copy `.env.example` to `.env`
```
cp .env.example .env
```


### Start container services

If the container have been created before, the docker-compose will start the existing one.

**Staging**
```bash
docker-compose -f docker-compose.staging.yml up -d
```

**Production**
```bash
docker-compose -f docker-compose.production.yml up -d
```


### Stop container services
Stop all the services without destroy the container
**Staging**
```bash
docker-compose -f docker-compose.staging.yml stop -d
```

**Production**
```bash
docker-compose -f docker-compose.production.yml stop -d
```

### Destroy containers
**Staging**
```bash
docker-compose -f docker-compose.staging.yml down -d
```

**Production**
```bash
docker-compose -f docker-compose.production.yml down -d
```

### Database Directory

* `$(pwd)/database/prd/data` ~-> production database host data
* `$(pwd)/database/stg/data` ~-> staging database host data

### Access on MongoDB express Dashboard

**Staging**
```
http://localhost:8001
```

**Production**
```
http://localhost:8002
```

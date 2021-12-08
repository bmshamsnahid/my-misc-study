### Install

---

```docker
docker run -d -p 27017:27017 -v ~/mongo-local:/data/db --name mongo-local mongo:latest
```

**-p**: Doing the port mapping.

**-v**: Doing volume mapping. Even if the mongodb instance is shut-down, the data will be persisted in local machine.

**--name**: The container name.

**mongo:latest**: Using the latest mongoDB image for the container.

### Run MongoDB

---

```bash
docker start mongo-local
```

### Check The Database

---

First go to the container,

```docker
docker exec -it mongo-local bash
```

This will open the bash inside the mongodb.

We can run `mongo` to open the db console,

```bash
mongo
```

### Restore The Database

---

Make sure `mongo-tools` are installed in your system. This tool includes the `mongodump` and `mongorestore` to dump or restore the database.

Go to the directory that contains the `dump` file and restore the database by,

```bash
mongorestore -h localhost:27017
```

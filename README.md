# mongodb-guide
Repository with practical guide from Max Swarzmuller at udemy at MongoDB.

## Starting MongoDB
### Starting db server
```
  mongod --dbpath <path>/data --logpath <path>/logs/mongo.log
```
Or
```
mongod --dbpath $HOME/data
```

### Reopen db server
```
mongod --dbpath <path>/data --logpath <path>/logs/mongo.log --logRotate reopen --logappend
```

### Starting Mongo shell
Old Shell
```
  mongo
```
Newer Shell
```
  mongosh
```

## Rotating log file
```
use admin
```
```
db.adminCommand({ logRotate: "server" })
```

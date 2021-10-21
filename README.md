# MONGO-API

This is a NodeJS based REST API system and works with [mongodb](https://mongodb.org/)

## Install:
```bash
git clone https://github.com/jaysixnine/mongo-api
cd mongo-api
npm install
```

## Before Start:
Create a "database" directory under /src and an index.js file

The src/database/index.js should contain:
```js
const mongoose = require('mongoose');
mongoose.connect(`mongodb+srv://<username>:<password>@<database>.qbogc.mongodb.net/<databaseName?retryWrites=true&w=majority`); // if your mongodb is running on cloud
mongoose.connect(`mongodb:localhost/<databaseName>`) // if your database is running locally
mongoose.Promise = global.Promise;
module.exports = mongoose;
```

## This project contains:
>Registration with method POST (accept json type)
---
>Authenticate system with token on header
---
>Integration with mongodb
---
License: [MIT](https://en.wikipedia.org/wiki/MIT_License)

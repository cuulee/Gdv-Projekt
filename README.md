# Visualization project hexbike



## Documentation
The full Documentation can be found here:
https://tillnagel.github.io/gdv-ws2017-website/projects/HexBike/

## Installation

Clone the repository:

```
git clone https://github.com/haChristopher/Gdv-Projekt
```
then move to the directionary "Visualisierung" and run npm install:

```
cd Gdv-Projekt/Visualisierung
npm install
```

### Setup database 

Use the dump file ```Dump20180116.zip``` and import it into a mysql database.
For the import you can either use the command line:

```
sql -u username -p database_name < file.sql
```

or you can use the mysql workbench.


Then go to Gdv-Projekt/Visualisierung/routes/sqlDatabase.js and change the sql connection settings with your database settings:

```
var connection = mysql.createConnection({
    "host": "localhost",
    "user": "root",
    "password": "root",
    "port": "3306",
    "database": "gdv_nextbike",
    "timezone": 'utc'
});
```

### Run project

To the run the project run:

```
node app.js
```

then go to localhost:3000

### Dependencies


Python 3.4.4: https://www.python.org/downloads/release/python-344/

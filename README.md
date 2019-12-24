# docker-compose-mysql-with-adminer
Local MySQL Docker = Docker Compose + MySQL + Adminer

## Usage

On folder that contains `docker-compose.yml` type one of this.

```
// non detach mode
docker-compose up
```
or
```
// detach mode
docker-compose up -d
```

To shutdown database without delete the data that already created

```
docker-compose stop
```

To shutdown database and delete all data that already created
```
docker-compose down
```

It will spin the MySQL latest version, expose port to host at 3306 and ready connection via Adminer.

## MySQL credential

- Username: root
- Password: rootpassword

## How to connect to MySQL

### Adminer
Go to http://localhost:8080

### Command Line
Make sure you have MySQL client installed and `mysql` command in CLI available.

```
mysql -uroot -prootpassword -h 127.0.0.1
```

or

```
mysql -uroot -prootpassword --protocol=TCP
```

Enjoy your local MySQL database server for testing purpose.

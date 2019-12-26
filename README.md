# docker-compose-mysql-with-adminer
Local MySQL = Docker + Docker Compose + MySQL Docker image + Adminer Docker image

## Usage (start server)

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

It will spin the MySQL latest version, expose port to host at 3306 and ready connection via Adminer.

## Usage (stop server)

To shutdown database without delete the data that already created

```
docker-compose stop
```

To shutdown database and delete all data that already created
```
docker-compose down
```

## MySQL credential

- Username: root
- Password: rootpassword

## How to connect to MySQL

### Via Adminer
Go to http://localhost:8080

### Via command line
Make sure you have MySQL client installed and `mysql` command in CLI available.

```
mysql -uroot -prootpassword -h 127.0.0.1
```

or

```
mysql -uroot -prootpassword --protocol=TCP
```

Enjoy your local MySQL database server for any purpose you want, for me this setup is fine for testing purpose.

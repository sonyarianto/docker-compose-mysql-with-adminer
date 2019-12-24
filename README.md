# docker-compose-mysql-with-adminer
Local MySQL Docker = Docker Compose + MySQL + Adminer

## Usage

```
docker-compose up
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

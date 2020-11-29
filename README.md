# vapor-hello

## ローカルにPostgreSQLを立てる

```shell

docker run --rm -d \
    -p 5432:5432 \
    -e POSTGRES_PASSWORD=mysecretpassword \
    -d postgres

```

## PostgreSQLに接続する

```shell
postgres
psql
```

### PostgreSQLにアプリケーション用のユーザ作成

```shell
create user vapor;
\password vapor
```

### PostgreSQLにアプリケーション用のデータベース作成


```shell
create database vapor;
```

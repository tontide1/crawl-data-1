# crawl-data-1
Crawl data form F1 motor website (Lab on Intro data engineering)

## 1. Prepare

- Install **Air-flow** and **My-SQL** images
```
docker pull mysql
docker pull apache/airflow:2.8.3
docker run --name mysql-db -e MYSQL_ROOT_PASSWORD=root -p 3333:3306 -d mysql:latest
docker run --name airflow --link mysql-db:mysql-db -d -p 8080:8080 apache/airflow:2.8.3
```

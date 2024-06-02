module cmd/go-api-sample-todo

go 1.22.3

1. run mysql db
docker run --name payment-db -e MYSQL_ROOT_PASSWORD=root -d -p 3306:3306 mysql:latest
docker exec -it payment-db bash
mysql -u root -proot
CREATE DATABASE Payment;
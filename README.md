module cmd/go-api-sample-todo

go 1.22.3

1. run mysql db
docker run --name product-db -e MYSQL_ROOT_PASSWORD=root -d -p 3306:3306 mysql:latest
docker exec -it product-db bash
mysql -u root -proot
CREATE DATABASE products;

go mod init github.com/marwenbhriz/go-rest-api
go get .
go get github.com/marwenbhriz/go-rest-api/controllers/productcontroller
go get github.com/marwenbhriz/go-rest-api/models

go get gorm.io/driver/mysql
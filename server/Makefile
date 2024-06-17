postgresinit:
	docker run --name postgres15 -p 5433:5432 -e POSTGRES_USER=root -e POSTGRES_PASSWORD=password -d postgres:15-alpine

postgres:
	docker exec -it postgres15 psql

createdb:
	docker exec -it postgres15 createdb --username=root --owner=root go-chat

dropdb:
	docker exec -it postgres15 dropdb go-chat

migrateup:
	migrate -path db/migrations -database "postgres://chatgo_user:VT3PlSTZ8QT3BIpS1WOkFPoH2yamiND6@dpg-cpnh0nuehbks7387kfo0-a:5432/GoChat?sslmode=disable" -verbose up

migratedown:
	migrate -path db/migrations -database "postgres://chatgo_user:VT3PlSTZ8QT3BIpS1WOkFPoH2yamiND6@dpg-cpnh0nuehbks7387kfo0-a:5432/GoChat?sslmode=disable" -verbose down

.PHONY: postgresinit postgres createdb dropdb migrateup migratedown
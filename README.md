mvn clean package

docker-compose down

//
creating image
cd kafka-producer
docker build -t kafka-producer .


//creating jar file images
cd flink-processor
mvn clean package 
docker build -t flink-processor .

//
cd ..
docker-compose up --build -d

//docker-compose up -d

//
for kafka-producer

docker ps -a
docker logs --tail 2000 <id>

//
docker exec -it postgres psql -U postgres -d postgres
\dt (relations)
select * from weather;
-------------------------------------
docker-compose down
--------------------------
$docker rm -f

docker rm -f $(docker ps -aq)



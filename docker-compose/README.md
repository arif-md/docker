1. replace aws_account_id in my-app-compose.yaml with the real AWS Account ID
2. docker compose -f mongo-compose.yaml up -d
3. create the DB by name "my-db" by visiting the URL : http://localhost:8080/
4. select my-db and create collections by name "users"
5. access the applicaiton at http://localost:3000/
6. docker ps
7. docker compose -f mongo-compose.yaml down

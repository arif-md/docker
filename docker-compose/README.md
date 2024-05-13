TODO : replace aws_account_id in my-app-compose.yaml with AWS Acc ID

docker compose -f mongo-compose.yaml up -d
visit : htt:localhost:8080
docker ps
docker compose -f mongo-compose.yaml down

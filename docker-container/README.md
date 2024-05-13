docker build -t my-app:1.0 .
docker run my-app
docker image list
docker rm <container-id or name>
docker rmi <image-id>

---------------------------------------------------
Pushing to remote private repository using AWS ECR
---------------------------------------------------
1. Create ECR repository on AWS.
  Note: Check the following values in ECR repository create page.
2. aws configure
3. aws ecr get-login-password --region region | docker login --username AWS --password-stdin aws_account_id.dkr.ecr.region.amazonaws.com (Note: copy the command from AWS account after creating the ECR registry)
4. docker build -t my-app .
5. docker tag my-app:latest aws_account_id.dkr.ecr.region.amazonaws.com/my-app:latest 
6. docker push aws_account_id.dkr.ecr.region.amazonaws.com/my-app:latest
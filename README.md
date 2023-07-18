# hello-node
# step-by-step how to create an image until it will be deployed to AWS ECR
## Create git hub repository for this assignment: 3.5-container
### 1. create this repository with .gitignor : node
## Create a Repo in ECR
### 1. login to aws, goes to ECR service
### 2. create repository with name renpeng, leave others by default; make sure it is private.
### 3. : "git clone git@github.com:su-ntu-ctp/6m-cloud-3.4-cloud-native-application-containerization-i.git" this is just to download the example app files.
### 4. copy the files in subfolder: hello-node-pp,to my own folder. 
### 5. run "npm install"
### 6. push everthing to githup repo: 3.5-container 
## Run ECR commands at local
### 1. Authentication / Authorization to ECR
### can just copy the command from aws ECR console, under the ECR repo name: renpeng, click : view push command" and copy command 1: aws ecr get-login-password --region ap-southeast-1 | docker login --username AWS --password-stdin 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com
### 2. from same location as command 1, copy command 2: docker build -t renpeng .
### 3. copy and run command 3: docker tag renpeng:latest 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/renpeng:latest
### 4. copy and run command 4: docker push 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/renpeng:latest



# How_To_push_docker_Images_In_GCP :

#### Step 1 : setup the docker
- link : https://docs.docker.com/engine/install/ubuntu/ 
- sudo groupadd docker
- sudo gpasswd -a $USER docker

#### Step 2 : check docker images
-Docker

#### step 3 : docker login 

#### step 4 : docker pull username/project_name
#### step 5 : check the docker images using:
- docker images
#### step 6 : Check the gcloud project list
- gcloud projects list
#### step 7 : change the file pattarn.
- docker tag Docker_username/docker_project_name gcr.io/project_id/project_name:v1
- Example : docker tag musa/docker_project_name gcr.io/test-gpu/dress_api:v1
- Example : docker tag cavid101/dress_api:latest gcr.io/ai-project/dress_api:v1

#### Step 8 : check docker images
- docker images

#### step 9 : Push the docker Images 
- docker push gcr.io/test-gpu/project_name
- example: docker push gcr.io/ai-project-28721/dress_api

#### step 10: If you don't get permission use this
You don't have the needed permissions to perform this operation, and you may have 
invalid credentials. To authenticate your request, follow the steps in: https://cloud.google.com
/container-registry/docs/advanced-authentication

- gcloud auth configure-docker

#### step 11 : Push the docker Images again 

- docker push gcr.io/test-gpu/project_name

#### Step 12 : go to cloud and search Container Registry and select your project 

### link :
- Deploying a containerized web application: https://cloud.google.com/kubernetes-engine/docs/tutorials/hello-app
- Kubernetes Engine (GKE) cluster GPUs : https://cloud.google.com/kubernetes-engine/docs/how-to/gpus#gcloud

# Dockerized Go app on GCP Compute Engine

Deploying a simple dockerized golang application

## Getting Started

These instructions will help you deploy a simple GO app on Compute Engine

### Prerequisites

* Docker
* Nginx
* Git

## Deployment steps

1. Create VM
 
	gcloud compute instances create VM_NAME \
	[--image IMAGE | --image-family IMAGE_FAMILY] \
	--image-project IMAGE_PROJECT

2. Clone git repo

	git clone https://github.com/ma0456/operation.git

3. Build your docker image

	docker build -f /path/to/docker/file

4. Run your docker image

	docker run -p 8080:3000 "yourimagename"

## External links

* More about Docker: https://docs.docker.com/
* More about Go: https://go.dev/doc/
* More about Nginx: https://nginx.org/en/docs/ 
 

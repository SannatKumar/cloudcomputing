# Hands on With Docker

Docker is an open source platfrom for building, deploying and managing containerized applications.

For Example: microservices architecture.

MicroService Architecture: The feature are deployed as different services as opposed to monolithic architecture where everything together is a application.  

Docker helps to make server and database libraries and dependencies portable, extremely light, and totally isolated and independent.
No issues like working in local and not working in Production.  

# Docker: Use Cases

-- Modernization from "traditional" to Microservices applications.  

"if a container fails, only part of the application will be unavailable."  

"New deploys without affecting other componenents/services."  

-- Deployment Pattern
"Docker images are built using definition files."  

--Similar Environments

"Docker runs anywhere, anytime."  
"You just need Docker installed."  

*** Modern applications make use of Microservices Architecture ***

Terraform is the evolution of the infrastructure. Docker is the Evolution of the Applications.

# Virtual Machine  

Hardware --> Hypervsior --> Virtual Machine--> Operating System--> Application--> Libraries & Dependencies.

Each VM has:
App, OS, Kernel, Libs abd Deps
-- Higher resource utilization(OS/Kernel)
-- Higher Disk Space(GB)
-- Boot up: minutes

# Docker  

Hardware --> Operating System --> Docker --> Container --> Application --> Libraries & Dependencies.

Each Container has:
App, Libs and Deps
--Lower resources utilization(Only small part of the kernel).
--Lower disk space(MB)
--Boot up: seconds

# Hands-on with Docker on Cloud.

Requirement: Needs a proof of concept to deploy the application(that use to run in virtual machine) in top of containers in Google Cloud.

Use VS Code.  
First Create A docker file with the specification of the image that is going to provision a container.
We need a application file.  

Docker file and application file is used to create a docker image.

Docker image is a pack that will have a application file and libraries that is required to run a different application inside a conatiner.  

In order to create a image, we need command,  
we need to build.
$ docker build  
$ docker push  

Docker build is going to create a image. Once the image is created we are going to push the image to Container Registry on Google cloud.  
Container Registry is just like a repository where you can store your docker images.  

Docker images is used to deploy the application, For that we run cloud run. Cloud Run(Completely serverless service from Google) is a service tha allows us to deploy the applications 
without managing the infrastructure.  





















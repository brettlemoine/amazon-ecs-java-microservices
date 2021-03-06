## Introduction
### Java Microservices Deployed on EC2 Container Service

Containers are a method of operating system virtualization that allow you to run an application and its dependencies in resource-isolated processes. Containers allow you to easily package an application's code, configurations, and dependencies into easy to use building blocks that deliver environmental consistency, operational efficiency, developer productivity, and version control. Containers can help ensure that applications deploy quickly, reliably, and consistently regardless of deployment environment. Containers also give you more granular control over resources giving your infrastructure improved efficiency.

Running a single container on a single server is easy. ECS is a cluster management service that helps you manage a group of clusters through a graphical user interface or by accessing a command line. With ECS you can install, operate, and scale your own cluster management infrastructure. With simple API calls, you can launch and stop Docker-enabled applications, query the complete state of your cluster, and access many familiar features like security groups, Elastic Load Balancing, EBS volumes, and IAM roles. You can use Amazon ECS to schedule the placement of containers across your cluster based on your resource needs and availability requirements. You can also integrate your own scheduler or third-party schedulers to meet business or application specific requirements.

This is a reference architecture that shows the evolution of a Java application from a monolithic application that is deployed directly onto instances with no containerization or orchestration, to a containerized microservices architecture orchestrated using Amazon EC2 Container Service.

We will take the [Spring Pet Clinic](https://github.com/spring-projects/spring-petclinic) as the base to extend from.
A high level architecture of PetClinic app is as follows,
![alt text](https://github.com/awslabs/amazon-ecs-java-microservices/blob/master/images/PetClinicApp.png)

So lets get to it,
1. [Part One: Moving existing Java Spring application to a container deployed using ECS](https://github.com/awslabs/aws-java-microservice-refarch/blob/master/1_ECS_Java_Spring_PetClinic)
2. [Part Two: Breaking the monolith apart into microservices on ECS](https://github.com/awslabs/aws-java-microservice-refarch/tree/master/2_ECS_Java_Spring_PetClinic_Microservices)
3. [Part Two: Create a continuous integration and continuous delivery](https://github.com/awslabs/aws-java-microservice-refarch/tree/master/2_ECS_Java_Spring_PetClinic_CICD)

## Prerequisites

You will need to have the latest version of the AWS CLI and maven installed before running the deployment script.  If you need help installing either of these components, please follow the links below:

1. [Installing the AWS CLI](http://docs.aws.amazon.com/cli/latest/userguide/installing.html)
2. [Installing Maven](https://maven.apache.org/install.html)
3. [Installing Docker](https://docs.docker.com/engine/installation/)
4. [Installing Python](https://www.python.org/downloads/)
5. [Installing JQ](https://stedolan.github.io/jq/download/)

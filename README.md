# kubernetes-gcp
    A container Ochestration tool.

<hr><br>

### Contents:
 ### 1.   [Introduction](/README.md#introduction)
 ### 2. [Architeture](/README.md#architeture)

<hr><br>

## 1. Introduction 

 k8 is a container archestration tool, which helps to manage container based application, to deploy, manage, and secure the application. It provides several features like storing the secrets, exposing the container with external and internal api service, enables the container based service to interact with private IPs  without going through the internet, hence enabling the fast communication.

<hr><br>

## 2. Architecture

Historically we deployes application on single server or vertual machines where we have hyperviser installed on servers, this way we can isolate the virtual invironment where application is running. This helps us to manage app independently on the underlying operation system. 

    Hyperviser
![Vitual machine based architecture](/docs/images/hyperviser.jpeg)

Since drawback of such system was even for small application, VM needs to be configured which is not effectively utilising the resources. 

To overcome this challenge , then came the concept of containerisation of an application, where we bundle an apllication to a lightweight container which is easy to deploy and spinup on any server where docker is availble.  

    DOCKER

![docker based application](/docs/images/docker.jpeg)

Docker based application is easy to maintain and deploy. However in production server where several of such container based application is deployed and running, so managing and effectively running them is challenging, which is why a Container Ochestration tool such as K8 is needed. This way we can effectively manage, deploy and securely access the applications and exposes only those services which needs  public access otherwise all containers comminucates through private network within K8 cluster.  

    K8 architecture
![k8-architecture](/docs/images/kubernetes-arch-01.jpeg)
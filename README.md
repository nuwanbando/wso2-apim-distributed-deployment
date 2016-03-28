### This repository contains API Manager 1.10.0 distributed deployment for PoC / Demo purposes

Following instructions will help you to setup the deployment

1. Clone the repository to your local file system
2. navigate into the parent directory (wso2-apim-distributed-deployment)
3. Execute ``` docker-compose up -d ```

This will setup 

* A mysql server (container) with apimdb / userdb / regdb
* A container with apim-gateway / apim-keymanager / apim-store / apim-publisher

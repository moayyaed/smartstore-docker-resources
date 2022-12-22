# Running Smartstore with MySQL in Docker
## Prerequisites
 * [Docker](https://www.docker.com/) 
 * [Docker compose](https://docs.docker.com/compose/install/) (Docker Desktop for Windows or Mac includes Docker Compose, install this, if you are using a Linux OS)   
## Download and Run Docker Compose File
* Download the [Docker Compose file](https://github.com/smartstore/smartstore-docker-resources/blob/main/docker-compose.yml)
* Change to the directory where you saved the file
* At the command line, run `docker compose up`
## Install Smartstore
* Enter `http://localhost` into your browser
* The Smartstore setup wizard will open
## Input fields during setup
### Store Information
+ **Admin user email**: Username for the Shop Admin
+ **Admin user password**: Password of the Shop Admin
+ **Confirm the password**: Confirmation of the Shop Admin password
 


![Database information](https://www.smartstore.com/de/news/images/smartstore-installation-store-info-640.png)  
### Database information
+ **Database system**: Specifies which database system is used, we choose `MySQL` here.
+ **Connection**: Here you can choose between entering the individual connection string values and the connection string as a whole. We select `Enter connection values`
+ **Servername**: The host name or IP of the database server. Here we enter `mysql`
+ **Database name**: Name of the database. This is newly created and the name can be freely chosen, e.g. `db-smartstore`
+ **Authentication**: Here you can choose between the available authentication methods. MySQL only offers `SQL server authentication` here
+ **Username**: Username for the MySQL server. In this example, we use `root` for simplicity. 
+ **Password**: The password of the root user is `Smartstore2022!`



![Database information](https://www.smartstore.com/de/news/images/smartstore-installation-db-info-640.png)  

### Options
+ **Primary language**: Here you have the possibility to select a store language. Later more languages can be installed.
+ **Media storage**: Here the selection is made whether the media should be stored on the file system or in the database. The default setting should remain.
+ **Create sample data**: Determines whether sample data is created. For testing, this option should be enabled.  



![Options](https://www.smartstore.com/de/news/images/smartstore-installation-options-640.png)

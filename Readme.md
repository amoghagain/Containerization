﻿![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.001.png)Containerization 

**Containerization** in Docker refers to the process of packaging an application and its dependencies into a standardized unit called a **container**. This approach allows developers to create, deploy, and run applications consistently across various computing environments.

Tasks :

1. Task:
   This repository contains the Docker setup for launching a web application along with a separate database container. The application is accessible on `localhost:8080`, while the database is isolated within a Docker network.

   The Rails app is locally directed and dockerfile and docker-compose are updated as in the folder my-app-task and accordingly we can containerize the application using the below commands:
   ![image alt](https://github.com/amoghagain/Containerization/blob/f3d362374975b4a65e598bf6ad5ed52a1db0872e/bonus0.PNG)



   ![image alt](https://github.com/amoghagain/Containerization/blob/d6274d03e43eb2181ab5f962423bd5db2a97ad72/bonus01.PNG)

1. Bonus 1:

   An **Nginx container** refers to a Docker container that runs the Nginx web server. Nginx is a high-performance web server and reverse proxy server that can also be used as a load balancer, HTTP cache, and more. Running Nginx in a container allows you to easily deploy, manage, and scale your web applications or services in isolated environments.

   A **reverse proxy** is a server that sits between client devices (like web browsers) and backend servers (like application servers). It forwards client requests to the appropriate backend server and then sends the server's response back to the clients. This setup can help improve the performance, security, and reliability of web applications. Mostly helps in load balancing.

   We have an additional nginx file created and bought into implementation for this as the above folder my-app-bonus-1 explains about it.


   ![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.004.png)


   ![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.005.png)



   ![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.006.png)

1. Bonus-2 

   This task is similar to the above one but we are trying to launch multiple rails containers connecting to a single database.

   The above folder ‘my-app-bonus-2’ explains this.

   ![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.007.png)




   ![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.008.png)

   ![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.009.png)



   ![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.010.png)

1. Bonus-3 :

   The last task involves persistence:

   Persistence in Docker refers to the ability to keep data across container restarts and removals. By default, data stored in a Docker container is ephemeral, meaning it disappears when the container stops or is removed.

   This can be handled using volumes in a better way

**Data Persistence**

- **Database Data**: The MySQL database data is stored in the db\_data volume, ensuring that your data persists across container restarts.
- **Nginx Configuration**: The Nginx configuration file is mounted from the local filesystem, allowing you to modify it without needing to rebuild the container.

This setup enables you to run a web application with a MySQL database using Docker, ensuring that important data and configurations persist even when containers are stopped or removed. You can easily manage your application with Docker Compose, making it straightforward to start, stop, and monitor your containers.

![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.011.png)





![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.012.png)





![](Aspose.Words.7bdc1be7-b65b-44c6-90f1-ba100b872425.013.png)
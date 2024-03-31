## Docker Compose Project build using Flask and using Nginx as Loadbalancer
- This is basic flask based web application  to demonstrate the Docker compose concept
- So what is docker compose? so , Docker compose is tool for defining and running multi-container Docker applications. with compose we use a yaml file to configure our
  application services.
- Compose is work on all envirenment production , staging development, testing as well as workflow also.
- The key feature's of docker compose :
   1. Have Multiple isolated environment on a single host .
   2. Preserve volume data when container are created .
   3. Only recreate's the container that have changed .
   4. Supports variables and moving a composition beetween environments.
      
### Project setup-
-  First , clone this repository to your system.
-  I have coded the docker-compose file in .yaml format.
-  So type **docker-compose Up** command to start application.
-  In this project we are using flask based Wed API , Nginx server and redis as a backend database.

### Use of Nginx server to enable scaling in docker compose
- We are using nginx web servers as loadbalancer for scaling of our application.
- For this task we have setup nginx.conf file.
- After compliting the setup follow below command.
   ```
   docker-compose scale web=5
   ```
- Here web is name off a service and 5 number of containers to be scaled.
- The Nginx act as proxy server to allow our application to scale.
  
  


 

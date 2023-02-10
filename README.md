# Node-JS and mongoDb with Docker configuration
Project overview: 
    Simple project which helps users to manange album which includes all types of files.
    A user can upload with an expiry date and can give access to other users to view and download his album.
Docker:
To start with docker i have created a DockerFile which will create image for this project
There are few commands with comments in it please see the file 
After creating the DockerFile Please run this command
     docker build -t <name_for_image> .
     -t represents tag name
     . represents the current directory (go to the directory where the Dockerfile is located)
Then after creating docker-image create docker-compose.yml file in same directory
I have define our services/containers inside this file. 
When creating a docker-compose file, the .yml extension is a must.
Please see this file for more information
    Then run docker-compose up
And boom if everything is fine your services are up inside the container



Commands flow
npm i 
create .env copy from .env.example
docker build -t <name_for_image> .
docker-compose up
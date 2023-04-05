- Gist for setting up styling on your powershell https://github.com/romkatv/powerlevel10k#manual-font-installation
# Docker run commands
- -p is to specify the ports for the container and it goes localHost:containerHost -p 3000:80 means that to hit the container host on port 80 we need to go through localhost 3000
- --name lets you name the container that will be ran
- -d runs it detached 
- --restart let you say when the container should restart it self. 
- -e is used to specify environment variables
- -v adds volumes 

# Docker Compose
- The spacing in yml is important so make sure things are indented correctly.
- You dont need "" when writing in yml
- adding an environment: section will allow you to set diffrent environment variable as name value pairs.  
- There might be a docker-compose.override.yml that is used to override setting of the docker compose which in some cases can be useful. 
- A ports: section in the yml can allow you to map more ports with the same format as the -p  command from docker run
- Docker compose can have multiple services defined inside of the services section but make sure to pay attention to the indentation.
- You can use the depends_on: keyword to tell what services depend on each other so that the services can start up in order
- You can also specify what networks each service is apart of inside of the yml. 
# Nginx 
To make a nginx image you will need to a dockerfile that gives you the base image and then you also need a nginx config file for nginx as shown in the video. 

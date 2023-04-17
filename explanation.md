## BASE IMAGES
### Client and Backend
I used alpine which is much smaller in size than most distribution base images and thus leads to much smaller images in general.

### Database 
I used mongo which is the only available image for Mongo Database.

## DOCKERFILE DIRECTIVES
| Directive | Use   | 
| :-----: | :---: | 
| FROM | Specifies the parent image of our custom Docker image   | 
|WORKDIR |     Sets the working directory for any RUN, CMD, ENTRYPOINT, COPY and ADD instructions that follow it in the Dockerfile |
|RUN |         Executes commands during the image build time |
|COPY|         Copies new files or directories from <src> and adds them to the filesystem of the container at the path <dest> |
|EXPOSE |      Informs Docker that the container listens on the specified network ports at runtime|
|CMD    |      Provides a default initialization command that will be executed when a container is created from the Docker image |

## NETWORKING
I configured networks to ensure the containers communicate with each other.

## VOLUMES
Implemented volumes for data persistence

## GIT WORKFLOW
* Cloned the repository to my local repository
* Created a repository on my github account and added it as my remote repository
* Created the microservices and pushed changes to github.

## DOCKER IMAGE & CONTAINER NAMING 

I named all the images and containers to enable easy identification.

## SETUP INSTRUCTIONS
* git clone https://github.com/Dgichaba/yolo.git
* cd yolo
* docker-compose up --build
* Access App on http://localhost:3000

Application successfully running.
## LINK TO DOCKERHUB
[Link to Docker-Hub](https://hub.docker.com/search?q=dgichaba)

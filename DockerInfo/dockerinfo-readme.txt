Commands

Status of docker process to know running 
Docker ps

shows images:
docker images      

shows all containers including stopped:
docker ps -a      

To list all container ids
Docker ps -aq

Stop:
docker stop XXXX 
Xxxx is starting  letters(3 or 4…) of containerid

Stop all containers:
docker stop  $(docker ps -aq)

Remove conatiner:
docker rm  XXXX

remove all containers:
docker rm  $(docker ps -aq)


Remove image:
Docker rmi XXXX  (imageid)


remove all images:
docker rmi  $(docker images -aq)


Create app docker images n container:

Run:
docker-compose -f .\docker-compose.yml -f .\docker-compose.override.yml up -d

Stopping:
docker-compose -f .\docker-compose.yml -f .\docker-compose.override.yml down

Clean solution then will remove all docker container n images

Will remove all stopped containers/Images/unused things:
Docker system prune

Url: http://localhost:8000/swagger/index.html


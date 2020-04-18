 Build docker image:
 
 `sudo docker build -t myapp .`
 
 Here is code for running docker image:
 
 `sudo docker run -it -p 8081:8000 myapp`
 
 For creating netwrok:
 
 ` sudo docker network create mynetwork`
 
 connecting docker to network:
 
 `sudo docker run -it -p 8081:8000 --network=mynetwork myapp`
 
  `sudo docker run -it -p 5555:5432 --network=mynetwork postgres`

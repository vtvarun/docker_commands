# docker_commands
Docker is a light wieght OS level visualization that helps us to run projects without having the support softwares locally in your machine.

For example :
Let's say you are working on a java project and to develop a java project you need a lot of things like:
1. JDK (Java Development Kit)
2. IDE (IntelliJ or Eclipse)
3. Depenedencies
4. Application Code that you have written


If you run a docker command : docker run "name of project", it will run on your machine automatically:

Here are some docker commands :
1. docker run "imageName"  (it will download a docker image if not found locally, and run it as docker container)
2. Ctrl + C                (it will stop the docker container)
3. docker run -p 5000:5000 "imageName" (it will map the container port to the host port {hostport}:{containerport} -> container port will be seen on terminal or cmd or powershell
4. docker run -p {hostPort}:{containerPort} -d "imageName" (it will run the container in the back ground and you won't see anything, also you will get a container ID) CTRL + C, will not stop this container
5. docker logs containerID  (if you want to see the logs )
6. docker logs -f containerId (if you want to keep following the logs)
7. docker container ls (it shows the list of containers that are up and running)
8. docker run -p {differentHostPort}:{sameContainerPort} -d "imageName" (this will run another instance of the same image)
9. docker images (it will show all the images that are present locally)
10. docker container ls -a (it will show old containers as well)
11. docker container stop "containerID" (it will stop the container)
12. docker pull "imageName" (it pulls from registry to local machine)
13. docker search "imageName" (you can search for any image)
14. docker image history "imageID" (to get the history)
15. docker image remote "imageID" (to remove the image)

# Week 1 — App Containerization

In the last week, I did Architectural Diagrams, installed the CLI and setup alarm budgets.
Now, I started using the gitpod which is quite helpful. I created another branch named sumama-zaeem-patch-week-1 and will merge it when I complete week 1 tasks.
I learned the benefits of containerization
Learned about the DockerHub which is a container registry for images. I also learned about the OCI and also about linuxserver.io and jfrog
In this week's task, I will containerize the backend and create a docker file.
Just a random question, why does Dockerfile not have an extension? The reason is probably is that its easily to find by name and it just contains the instructions.
I also learned about the unionfile system and the layers in dockerfile
While typing command, -m tag is used for flask.
Then again, I learned about the environment variables such and their configuration
I also learned about the RUN vs CMD command and its difference, run is a layer whereas CMD executes when the container spins up.
then to further learn docker, i referred from the docker from udemy.
the learning and my journal is:
docker uses hte LXC containers.
kernel should be same, like for windows, it should be windows one, else it will create a vm to visualize.
Dockerfile is used to create images. I also learned about the community edition vs the enterprise edition.
I installed docker from the official repo.
In the second section, i learned about the docker commands.
docker run
docker ps 
docker stop  ... (name or ID is important for a container)
docker rm
docker images
docker rmi ... (make sure that no container is running)
docker pull

for example, if there is an docker image of an os, when it is run by using the docker command, it doesn't run because their is no process in it. it exits hence.
command:
Docker exec
runs command in a running container
other commands are
docker run -d ...
docker attach (ID)
docker ps -a
docker rm ...
image cannot be deleted unless container is removed.
Now getting the basic understanding about the working and commands and thee philospohy about the docker, I resumed the BootCamp.
latest is by default stage.
I run the backend flask aplication and wrote a dockerfile.

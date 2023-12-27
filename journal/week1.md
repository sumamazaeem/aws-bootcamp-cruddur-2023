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
when the application was run, it faced the problem as it was not showing anything on the public url. the reason was that the environment variables in the dockerfile were not setup. the ways to resolve this thing is using docker exec or using by attaching the shell to a running container

now I edited the app.py file and used -e to set the environment variable
the command will be
docker run -rm -p 4567:4567 -it -e FRONTEND_URL='*' -e BACKEND_URL='*' backend-flask

Then I installed the npm in the frontend folder.
I write a dockerfile and make dockercompaose in the rootfolder.
what is meant by dockercomposee, this command rund the both containers simulanesusly.

Week-1 Container Pricing by Chiraj Nayar.
I learned about the pricing about the codespaces, cloud9 and cloudtrail.
I learn about the container first strategy
docker and host configuration
securing images
secret management
application security
data security
monitoring containers
complaince framework

I also learned about the container best practices
1. keep host and docker updated to the latest securit patches
2. docker daemon and containers should run in non-root user mode
3. image vulnerability scanning
4. trusting a private vs public image registry
5. no sensitive data in docker file or images
6. use secret management service to share secrets
7. read only file system and volume for docker
8. seperate databases for long term storage
9. use devsecops practices while building application security
10. ensure all code is tested for vulnerabilities before production use

I also learned about the snyk opensource security which automatically find and fix vulnerabilities in the code.
then I learnt about the AWS secret manager and how it is used.
Alternatively, Hashicorp valut can be used for similar purpose
For image vulnerability;
Amazon Inspector can be used which integrates with AWS Ecosystem such as scanning ECS, EC2, ECR

Then I installed Docker on Ubuntu, installing docker engine and then docker desktop.
I followed the official docker compose getting started tutorial.
I learned nano and vim for learning.
I run the container, wrote the docker compose file, attached the volume and removed the containers afterwards
for the opensource version, clair can be used

I learned about the openAPI, swagger, watched a few youtube videos and learned the concepts of openAPI

I learned about the DynamoDB local configuration

# Project06

# Project overview
In this project we will be dealing with Docker, Github Actions and DockerHub 
to make a webpage and to bulid and push a docker image to DockerHub

# installing docker 
You can install docker with the command "sudo yum update -y" and then the acually command is "sudo yum install -y docker" and the dependincies are the same based on which ones you want 

# how to build and run the container
its pretty simple first, create a Dockerfile (or you can base it on the sample one provided) and use a bunch of commands in the file itself such as 

[FROM ubuntu:latest

RUN apt-get update
RUN apt-get install -y python3 python3-pip

RUN pip3 install numpy \
    pandas \
    featuretools]

and then you can build an image with the command "docker build -t <image-name>  ." 
and the you can see all the images you have built by using the command "docker images" then you can run it by using the command "docker run -it <image-name>"
you can view your project by using your browser and go to ip and port and type in the port and ip you assigen to it 

# Creating a DockerHub public repo
creating a public repo was really not that hard just had to create an account and then type in the name of said repo then boom had a repo of my own

# Configure GitHub Secrets 
well the only 2 credentials needed is your dockerhub username and password and you can use other things as variables

well you can go down to the secret tab and add a name such as my secret name is BANANA_CREAM_PIE since they are my favorite desserts

not much to change in the Github Workflow 


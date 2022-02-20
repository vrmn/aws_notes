

Notes into my aws journey and a bit of networking
=====================================

Inspried by these OG's repo
https://github.com/open-guides/og-aws

Table of Contents
-----------------

**Purpose**
To explore a different way of writing notes
Specifically on AWS and some networking for another project 

Table of Contents
-----------------

**AWS**


first of all what I want is to leverage the GPU's provided by AWS so I have to figure out how to launch a GPU instance
1) Set hook yourself up with aws EC2 before anything else. https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/get-set-up-for-amazon-ec2.html
   .ppk or .pem for the key pair. since using WSL and Ubuntu for the most part in this project .pem seems more appropriate.https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstances.html
   Then create a security group thats acts as a firewall controlling what goes in and out of the instance.  
   for inbound SSH, HTTP and HTTPS
3) Then youre ready to connect to your instance. 

**Docker**
1) clone a repo that has an image and a container to run it
docker run --name repo alpine/git clone https://github.com/docker/getting-started.git

2) Build the image 
docker build -t docker101tutorial .

3) Run the container
4) docker run -d -p 80:80 --name docker-tutorial docker101tutorial


**Networking**


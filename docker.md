# docker notes

### deploy docker online
digitalocean.com
- create a droplet with docker to practice deploy
- add the created machine ip to /etc/hosts make it simple to reference it (ex: machineIp newLocalName)
- ssh root@newLocalName

### commands
- $ docker login (login to dockerhub -by default- to access available docker images)
- $ docker run <image> (create image and start the image. it will also download all required software for each layer)
- $ docker start <name|id> (start a stopped image)
- $ docker stop <name|id> (stop an image give its name or docker id)
- $ docker rm <name|id> (kill and remove a docker container)

- create a docker image, as a daemon (-p), with name web1 (--name web1), expose port 80 to port 8080 (-p 8080:80)
   - public docker image: tutum/hello-world
   - $ docker run -d --name web1 -p 8080:80 dockerImage

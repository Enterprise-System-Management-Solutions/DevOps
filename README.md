# DevOps
it's a training session for DevOps. 

docker install :
================
yum update 
sudo yum install -y yum-utils device-mapper-persistent-data lvm2
sudo yum install -y docker-ce docker-ce-cli containerd.io

systemctl enable docker
systemctl start docker
systemctl status docker

docker version

================

docker images            ---check any images 
docker pull nginx:latest ---pull any images
docker ps               --- check any running images 
docker ps -a            --- check any stop images 
docker run -p 8000:80 nginx  --- run any container 
docker rm a5311d712177     --- delete the  container

-------------run permanently-----------

docker run -d -p 8000:80 -v /root/nginx-html:/usr/share/nginx/html --name my-nginx nginx
docker stop my-nginx     ---stop container

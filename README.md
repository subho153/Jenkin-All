# Jenkin-All
Here I will upload all the Jenkin project, commands and all.

**First go to EC2 Instance**

**Install Ec2 instance**
![image](https://github.com/subha152/Jenkin-All/assets/51635202/38f513ac-4533-4bcc-b100-124c76449df0)




sudo apt update
sudo apt install openjdk-11-jre
java -version

sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
  
sudo apt-get update
sudo apt-get install jenkins


To check the process wheather jenkins installed or not : **ps -ef | grep jenkin**


**Docker Slave Configuration**

sudo apt update
sudo apt install docker.io

**Grant the permission to docker deamon jenkins user and Ubuntu user**
sudo su - 
usermod -aG docker jenkins
usermod -aG docker ubuntu
systemctl restart docker

**restart Jenkins**
http://<ec2-instance-public-ip>:8080/restart



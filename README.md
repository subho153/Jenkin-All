![image](https://github.com/subha152/Jenkin-All/assets/51635202/5fa103f6-4185-4d18-a6fd-eb65a1503a15)# Jenkin-All
Here I will upload all the Jenkin project, commands and all.

**First go to EC2 Instance**

**Install Ec2 instance**
![image](https://github.com/subha152/Jenkin-All/assets/51635202/072fc633-6d64-4e9e-a1e9-a02ab1f763c8)


sudo apt update
sudo apt install openjdk-11-jre
java -version

curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null


sudo apt-get update
sudo apt-get install jenkins

To check the process wheather jenkins installed or not : **ps -ef | grep jenkin**

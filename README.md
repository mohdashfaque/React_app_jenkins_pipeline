## Demo
https://youtu.be/OHyKaceFi8Q

## create reactjs app's jenkins pipline

## setup Jenkins on AWS EC2 Ubuntu 22.04 instance

# install java
```
sudo apt-get update
sudo apt-get install openjdk-11-jdk
java -version
```

# install jenkins
```
sudo curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee   /usr/share/keyrings/jenkins-keyring.asc > /dev/null
sudo echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]   https://pkg.jenkins.io/debian-stable binary/ | sudo tee   /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins

sudo systemctl start jenkins
sudo systemctl status jenkins
sudo systemctl enable jenkins
sudo cat /var/lib/jenkins/secrets/initialAdminPassword

```

# install nodejs and npm
```
sudo apt-get install -y curl
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install -y nodejs
```
# give the jenkins user the privilige of the root user (sudo.....)
```
echo "jenkins ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers
```

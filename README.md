# Jenkins-installation
### Install Java
```
sudo apt update
sudo apt install fontconfig openjdk-21-jre
java -version
openjdk version "21.0.3" 2024-04-16
OpenJDK Runtime Environment (build 21.0.3+11-Debian-2)
OpenJDK 64-Bit Server VM (build 21.0.3+11-Debian-2, mixed mode, sharing)

```
## Install Jenkins
### Method 1
```
sudo apt update
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins

```
### change port 8080 to another port
```
sudo vim /etc/default/jenkins
HTTP_PORT=8080 # change port
sudo systemctl restart jenkins
sudo systemctl status jenkins
```
### Method 2
```
sudo apt update
https://updates.jenkins.io/download/war/
wget https://updates.jenkins.io/download/war/2.500/jenkins.war
java -jar jenkins.war --httpPort=8082

**You have choice jankins version also port number

```

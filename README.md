# Jenkins--installation
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
https://updates.jenkins.io/download/war/
wget https://updates.jenkins.io/download/war/2.500/jenkins.war
java -jar jenkins.war --httpPort=8082

**You have choice jankins version also port number

```

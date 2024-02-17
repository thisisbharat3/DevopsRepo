```
sudo su -
yum update –y

# install git
yum install -y git

# install docker
yum install -y docker
systemctl start docker
systemctl enable docker



# install maven
sudo yum install -y maven

# install jenkins: 
wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo
rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key
yum upgrade -y
yum install jenkins -y
systemctl enable jenkins
sudo usermod -aG docker jenkins
systemctl start jenkins
systemctl status jenkins

#jenkins password
cat /var/lib/jenkins/secrets/initialAdminPassword

# install docker compose
curl -SL https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
sudo yum update -y

# install Ansible
amazon-linux-extras list | grep ansible
sudo amazon-linux-extras install ansible2 -y 

```

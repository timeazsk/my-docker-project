# My Docker Project

## Prerequisites

* Ubuntu 20.04
* [Install Docker](#install-docker) (Engine + Compose) 

## Install Docker

```bash
sudo apt-get install apt-transport-https ca-certificates curl tree software-properties-common -y
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg | apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
sudo apt-get install docker-ce docker-compose -y
```

## Manage Docker as a non-root user

```bash
sudo groupadd docker
sudo usermod -aG docker $USER
```

## Configure Authentication

Default credentials are `adminuser:adminpassword` \
You can set different credentials in `.htpaswd` file.

## Run Application

* Clone this repository
```bash
git clone https://github.com/timeazsk/my-docker-project.git
```

Change directory
```bash
cd my-docker-project
```

* Run command
```bash
docker-compose up –d
```

 > Application is started on http://localhost:80

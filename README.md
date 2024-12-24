# Smart Home

## 1 Homebridge Installation

### 1.1 OS
1. Settings:
 - Set hostname
 - Set username and password
 - Activate SSH through user
2. Install OS
   
### 1.2 Install docker

`curl -sSL https://get.docker.com | sh`

### 1.3 Add current user to docker group
`sudo usermod -aG docker ${USER}`

### 1.4 Check the docker group
`groups ${USER}`

### 1.5 Install docker compose dependencies
`sudo apt-get install libffi-dev libssl-dev`

`sudo apt install python3-dev`

`sudo apt-get install -y python3 python3-pip`

### 1.6 Install docker compose
`sudo pip3 install docker-compose`

### 1.7 Enable docker run with system startup through system service
`sudo systemctl enable docker`

### 1.8 Create homebridge directory
`mkdir /home/pi/homebridge`

`cd /home/pi/homebridge`

### 1.9 Create docker compose file
`nano docker-compose.yml`

### 1.10 Check containers
`docker ps`
or
`docker ps -a`

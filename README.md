# smarthome

## Installation

// OS
1. Settings:
 - Set hostname
 - Set username and password
 - Activate SSH through user
2. Install OS
   
// Install docker
curl -sSL https://get.docker.com | sh

// Add current user to docker group
sudo usermod -aG docker ${USER}

// Check the docker group
groups ${USER}

// Install docker compose dependencies
sudo apt-get install libffi-dev libssl-dev
sudo apt install python3-dev
sudo apt-get install -y python3 python3-pip

// Install docker compose
sudo pip3 install docker-compose

// Enable docker run with system startup through system service
sudo systemctl enable docker

// Create homebridge directory
mkdir /home/pi/homebridge
cd /home/pi/homebridge

// Create docker compose file
nano docker-compose.yml

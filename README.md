# Teleport-Server
#Setup
## Add the Teleport APT repository
sudo sh -c "echo 'deb https://deb.releases.teleport.dev/ $(lsb_release -cs) main' > /etc/apt/sources.list.d/teleport.list"

## Download the Teleport public key
wget -qO - https://deb.releases.teleport.dev/teleport.asc | sudo apt-key add -

## Update your package list
sudo apt-get update

## Install Teleport
sudo apt-get install -y teleport


# Guide-Devnet-Nexus-
# Guide to Running a Nexus Devnet Web Node

This guide will help you set up a Nexus Devnet Web Node using the official documentation.

## Prerequisites

Ensure you have the following installed on your system:
- Ubuntu (recommended)
- Docker & Docker Compose
- Git
- Terminal (Command Line Interface)

## Installation Steps

### 1. Clone this Repository
Open your terminal and run:
```bash
git clone https://github.com/Risxyiee/Guide-Devnet-Nexus-.git
cd Guide-Devnet-Nexus-
```

### 2. Install Docker & Dependencies
Run the following commands in your terminal:
```bash
sudo apt update && sudo apt install -y curl git
curl -fsSL https://get.docker.com | bash
sudo usermod -aG docker $USER
newgrp docker
```

### 3. Set Up Nexus Web Node
Use the terminal to execute:
```bash
docker run -d --name nexus-web-node -p 30333:30333 nexusofficial/web-node:latest
```

### 4. Verify the Node is Running
Check the running containers by executing:
```bash
docker ps
```

## Stopping & Restarting the Node
To stop the node:
```bash
docker stop nexus-web-node
```
To restart the node:
```bash
docker start nexus-web-node
```

## Conclusion
You have successfully set up a Nexus Devnet Web Node! For more details, check the [official documentation](https://docs.nexus.xyz/layer-1/network-devnet/web-node).

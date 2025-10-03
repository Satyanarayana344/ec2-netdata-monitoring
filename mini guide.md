# Monitor System Resources with Netdata on EC2

## Objective
Install and run Netdata on AWS EC2 Ubuntu instance to visualize system and app performance metrics.

## Tools
- AWS EC2 Ubuntu
- Docker
- Netdata (via official Docker image)

## Steps
1. Launch EC2 instance and open port 19999.
2. Install Docker:
sudo apt update && sudo apt install -y docker.io

Run Netdata:
sudo docker run -d --name=netdata -p 19999:19999 netdata/netdata

Access dashboard:
http://<EC2-PUBLIC-IP>:19999

Deliverables:
Netdata dashboard screenshot
Docker container running Netdata
Logs & metrics explored

Outcome:
Understand lightweight monitoring for servers and applications. 

I attach the screenshots how the netdata dashboard shows system monitor performances.

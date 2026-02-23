

# TASK 7 - Monitor System Resources Using Netdata

## Objective
Installed Netdata using Docker to monitor system performance.

## Tools Used
- Netdata
- Docker
- AWS EC2 (Ubuntu)

## Steps Performed
1. Installed Docker
2. Ran Netdata container
3. Opened port 19999
4. Accessed dashboard via browser

## Metrics Monitored
- CPU Usage
- Memory Usage
- Disk Usage
- Network Activity
- Docker Containers

Perfect 👍 Below is the **complete list of all commands used in TASK 7 – Netdata Monitoring Project** 


                                                  # ✅ 📌 All Commands Used in Netdata Project

# 1️⃣ Connect to EC2 / VM
ssh -i your-key.pem ubuntu@your-public-ip

# 2️⃣ Update system packages
sudo apt update -y

# 3️⃣ Install Docker
sudo apt install docker.io -y

# 4️⃣ Start Docker service
sudo systemctl start docker

# 5️⃣ Enable Docker on boot
sudo systemctl enable docker

# 6️⃣ Check Docker version
docker --version

# 7️⃣ Check Docker service status
sudo systemctl status docker

# 8️⃣ Pull and Run Netdata container
sudo docker run -d --name=netdata -p 19999:19999 netdata/netdata

# 9️⃣ Check running containers
sudo docker ps

# 🔟 Check all containers (running + stopped)
sudo docker ps -a

# 1️⃣1️⃣ View container logs
sudo docker logs netdata

# 1️⃣2️⃣ Stop Netdata container
sudo docker stop netdata

# 1️⃣3️⃣ Start Netdata container again
sudo docker start netdata

# 1️⃣4️⃣ Remove Netdata container
sudo docker rm netdata

# 1️⃣5️⃣ Remove Netdata image (if needed)
sudo docker rmi netdata/netdata

# 1️⃣6️⃣ Check system CPU usage (Linux command)
top

# 1️⃣7️⃣ Check memory usage
free -m

# 1️⃣8️⃣ Check disk usage
df -h

# 1️⃣9️⃣ Check Docker images
sudo docker images


# 🌐 Access Dashboard Command (Browser)


http://your-public-ip:19999

# 📂 Optional: Check Netdata Logs 

cd /var/log/netdata
ls


## Outcome
Successfully monitored real-time system metrics using Netdata.

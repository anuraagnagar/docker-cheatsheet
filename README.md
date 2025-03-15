### What is Docker? 🚀

Docker is an open-source platform that allows developers to automate the deployment of applications inside lightweight, portable containers. Containers package an application along with its dependencies, libraries, and configurations, ensuring it runs consistently across different environments.
Why Do We Use Docker?

    Portability – Run your application anywhere (local machine, cloud, or on-premise servers).
    Scalability – Easily scale applications up or down using container orchestration tools like Kubernetes.
    Dependency Management – Packages all dependencies inside the container, avoiding compatibility issues.
    Resource Efficiency – Uses fewer resources than traditional VMs since multiple containers share the same OS kernel.
    Fast Deployment – Containers start in seconds, making deployment quick and efficient.
    Isolation – Each container runs in an isolated environment, reducing conflicts between applications.

### **1️⃣ Basic Commands**
```
docker --version         # Check Docker version  
docker info              # Display system-wide information  
docker help              # List available Docker commands  
```

---

### **2️⃣ Working with Images**  
```
docker pull <image_name>          # Download image from Docker Hub  
docker images                     # List available images  
docker rmi <image_id>              # Remove an image  
docker tag <image> <repo>:<tag>   # Tag an image  
docker push <repo>:<tag>          # Push an image to Docker Hub  
```

---

### **3️⃣ Working with Containers**  
```
docker run <image_name>              # Run a new container  
docker run -d <image_name>            # Run in detached mode (background)  
docker run -it <image_name> /bin/bash # Run interactively  
docker ps                             # List running containers  
docker ps -a                          # List all containers  
docker stop <container_id>            # Stop a container  
docker start <container_id>           # Start a container  
docker restart <container_id>         # Restart a container  
docker rm <container_id>              # Remove a container  
```

---

### **4️⃣ Managing Container Logs & Processes**  
```
docker logs <container_id>       # View container logs  
docker top <container_id>        # Show running processes in a container  
docker inspect <container_id>    # Detailed container information  
docker stats                     # Live resource usage (CPU, memory, etc.)  
```

---

### **5️⃣ Working with Volumes (Data Persistence)**  
```
docker volume create my_volume      # Create a volume  
docker volume ls                     # List all volumes  
docker run -v my_volume:/data ubuntu # Attach volume to a container  
docker volume rm my_volume           # Remove a volume  
```

---

### **6️⃣ Docker Networks**  
```
docker network ls                      # List available networks  
docker network create my_network        # Create a custom network  
docker network connect my_network <container>  # Connect container to network  
docker network rm my_network            # Remove a network  
```

---

### **7️⃣ Building Custom Images (Dockerfile)**  
```
docker build -t my_image .  # Build image from Dockerfile  
docker tag my_image myrepo/my_image:v1  # Tag an image  
docker push myrepo/my_image:v1          # Push image to Docker Hub  
```

---

### **8️⃣ Docker Compose (Multi-Container Apps)**  
```
docker-compose up      # Start all services defined in docker-compose.yml  
docker-compose down    # Stop and remove all services  
docker-compose ps      # List running services  
```

---

### **9️⃣ Docker Clean-up Commands**  
```
docker system prune -a          # Remove all unused images, containers, and networks  
docker container prune           # Remove all stopped containers  
docker image prune               # Remove all dangling (unused) images  
docker volume prune              # Remove all unused volumes  
```

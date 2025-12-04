# 🚀 SRE / DevOps Learning Journey – Akshat Srivastava

![Docker](https://img.shields.io/badge/Docker-Learning-blue?logo=docker)
![DevOps](https://img.shields.io/badge/DevOps-SRE-green)
![GitHub](https://img.shields.io/badge/GitHub-Active-brightgreen)
![Cloud](https://img.shields.io/badge/Cloud-AWS-orange)

Welcome — this repository documents my hands-on journey to become a **Site Reliability Engineer / DevOps / Cloud Engineer**.  
I focus on practical labs, daily notes, Docker -> Linux -> CI/CD -> Terraform -> Kubernetes -> AWS -> Monitoring.

---

## 🧑‍💻 About Me
Hi, I'm **Akshat Srivastava**. I’m preparing for SRE / DevOps roles at product companies.  
I follow a disciplined, daily-practice approach and push all work here for accountability and to show real progress.

---

## 🛠 Core Skills & Tools

<p>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white"/>
  <img src="https://img.shields.io/badge/Terraform-623CE4?style=for-the-badge&logo=terraform&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white"/>
  <img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white"/>
</p>

---

## 📅 Progress (Daily Notes)

### ✅ Day 1 – Docker Setup & Basics
- Installed Docker Desktop  
- Concepts: Images, Containers, differences with VMs  
- Ran: `docker run hello-world`  
- Commands learned: `docker ps`, `docker images`, `docker run`  
- Notes: `/docker-basics/Day-1/`

### ✅ Day 2 – Docker CLI & Container Lifecycle
- Practiced: `docker run -d --name <name> -p host:container`, `docker stop`, `docker rm`  
- Port mapping: `-p 8080:80`  
- Exec into container: `docker exec -it mynginx /bin/bash`  
- Learned `ls`, `ls -la`, basics of container FS  
- Notes: `/docker-basics/Day-2/`

### 🔄 Day 3 – Docker Images & Layers (in progress)
- Image layers & copy-on-write explained  
- Commands: `docker history`, `docker inspect`  
- Built a small custom image and ran it  
- Notes: `/docker-basics/Day-3/`

---

## 📂 Repo Structure (how I organize work)





Each day folder includes:
- `notes.md` (explanations + commands)  
- screenshots (proof of work)  
- example `Dockerfile` / scripts if relevant

---

## 🔭 Roadmap (SRE / DevOps Focus)
**Phase A — Short-term (next 4 weeks)**
- Docker (deep) → Dockerfile best practices, multi-stage builds, image optimization  
- Linux essentials → file permissions, processes, journald/syslog, ssh, bash scripting  
- GitHub Actions → build & push Docker images automatically

**Phase B — Mid-term (1–3 months)**
- Terraform → IaC basics, modules, provisioning AWS resources  
- Kubernetes → pods, deployments, services, configMaps, secrets, ingress, helm  
- CI/CD (advance) → infra + app pipeline automation

**Phase C — Long-term (3+ months)**
- AWS (EKS, ECS, VPC, IAM, CloudWatch)  
- Monitoring & Observability → Prometheus, Grafana, Loki/ELK  
- High-availability & incident response practices  
- Final SRE Project: Terraform infra + EKS + GitHub Actions CI/CD + Monitoring

---

## 📘 Example — How to run the Day-2 demo locally
1. Build/run (already in repo day folder):
```bash
# from docker-basics/Day-2/
docker build -t akshat-nginx:day2 .
docker run -d --name akshat-nginx -p 8081:80 akshat-nginx:day2
# open http://localhost:8081



docker exec -it akshat-nginx /bin/bash
# inside: ls -la /usr/share/nginx/html
exit



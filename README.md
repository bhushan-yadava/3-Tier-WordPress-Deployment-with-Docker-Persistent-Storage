## 📌 3-Tier WordPress Deployment with Docker & Persistent Storage

This project demonstrates a 3-Tier architecture deployment of WordPress using Docker & Docker Compose with durable data storage.
It separates the application into three tiers:

Nginx (Web Server) → Handles client requests & static content.

WordPress (Application Server) → Runs WordPress PHP code.

MySQL (Database Server) → Stores WordPress data with persistence.

Persistent storage ensures that site data and database content remain intact even if containers are stopped or removed.



## 🚀 Features

3-Tier Architecture → Clear separation of Web, App, and Database layers.

Dockerized Setup → Reproducible deployment using Docker Compose.

Persistent Storage → MySQL & WordPress data stored in Docker volumes.

Custom Nginx Configuration → Optimized for WordPress + PHP-FPM.

Environment Variables → Secure credential handling via .env.

Ready for Cloud Migration → Can be extended to Kubernetes or AWS ECS.



## ▶️ How to Run

1️⃣ Clone the Repository
git clone https://github.com/<your-username>/3tier-wordpress-docker.git
cd 3tier-wordpress-docker

2️⃣ Start Services
docker-compose up -d

3️⃣ Access WordPress

Open http://localhost:8080
 in your browser.
You should see the WordPress installation screen 🎉

4️⃣ Stop Services
docker-compose down

5️⃣ (Optional) Remove Volumes
docker-compose down -v



## 📦 Persistent Storage

WordPress uploads & files → ./data/wp

MySQL database files → ./data/db

This ensures your website content and database are not lost when containers stop.

## 🛠️ Development with VS Code

Install VS Code extensions:

Docker (Microsoft)

Dev Containers (optional)

Run directly with VS Code tasks (.vscode/launch.json)

Debug containers & logs from the Docker Explorer in VS Code.




## ✅ Use Cases

Local development of WordPress sites.

Testing WordPress updates safely.

Understanding 3-tier containerized deployments.

Learning about persistent storage with Docker.



## 🔮 Future Improvements

Add phpMyAdmin for DB management.

Enable SSL/TLS (Let's Encrypt).

Extend deployment to Kubernetes (EKS/GKE).

Set up CI/CD with GitHub Actions.



## 📌 Technologies Used

Docker & Docker Compose

WordPress (PHP-FPM)

MySQL 8.0

Nginx (Alpine)

VS Code + Docker Extension

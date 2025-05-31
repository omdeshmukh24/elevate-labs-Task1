# 🚀 Node.js Demo App with CI/CD (GitHub Actions + Docker)

This is a simple Node.js web application that demonstrates an end-to-end CI/CD pipeline using **GitHub Actions** and **Docker**, with deployment on an **AWS EC2 Ubuntu instance**.

---

## 🛠️ Tech Stack

- Node.js
- Docker
- GitHub Actions
- AWS EC2 (Ubuntu)

---

## 📁 Project Structure

nodejs-demo-app/
├── app.js # Main Node.js application file
├── package.json # Node dependencies
├── Dockerfile # Docker instructions
└── .github/
└── workflows/
└── main.yml # CI/CD GitHub Actions workflow


---

## 🐳 Docker Commands (on EC2)

```bash
# Log in to Docker
docker login

# Pull the latest image
docker pull your-dockerhub-username/nodejs-demo-app:latest

# Run the container
docker run -d -p 3000:3000 --name nodeapp your-dockerhub-username/nodejs-demo-app:latest

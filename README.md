# 🚀 FastAPI + Docker + GitHub Actions (CI Only)

This is the **Day 1 DevOps Starter Project** 🎯  
It introduces the basics of modern DevOps with:

- ⚡ **FastAPI** → Lightweight Python framework for APIs  
- 🐳 **Docker** → Containerization to package apps  
- 🤖 **GitHub Actions** → Automating CI pipelines  
- 🧪 **Pytest + Flake8** → Testing & linting  

---

## 📂 Project Overview

- 📌 **FastAPI App** → A simple "Hello World" API  
- 🧪 **Pytest** → Unit test for the API  
- ✨ **Flake8** → Linting (PEP8 style check)  
- 🐳 **Docker** → Containerize the app  
- 🤖 **GitHub Actions** → Run lint + test + Docker build automatically on every push  

---

## ⚡ Getting Started (Local Setup)

### 1️⃣ Clone Repo
```bash
git clone https://github.com/your-username/devops-project-01-fastapi-docker-ci.git
cd devops-project-01-fastapi-docker-ci
2️⃣ Create Virtual Environment
bash
Copy code
python -m venv .venv
source .venv/bin/activate   # On Linux/Mac
.venv\Scripts\activate      # On Windows
3️⃣ Install Dependencies
bash
Copy code
pip install -r requirements.txt
pip install -r requirements-dev.txt
4️⃣ Run FastAPI App
bash
Copy code
uvicorn app.main:app --reload
Open in browser 🌐:

📖 Swagger UI → http://127.0.0.1:8000/docs

📝 ReDoc → http://127.0.0.1:8000/redoc

🧪 Run Tests & Lint
Run unit tests ✅

pytest -q
Run lint check ✨

bash
Copy code
flake8 app tests
🐳 Build & Run with Docker
Build Image
bash
Copy code
docker build -t fastapi-devops:1.0 .
Run Container
bash
Copy code
docker run -p 8000:8000 fastapi-devops:1.0
Visit → 🌐 http://127.0.0.1:8000

🤖 GitHub Actions CI
The CI pipeline (.github/workflows/ci.yml) runs on every push to main branch:

✅ Checkout code

✅ Install dependencies

✅ Run Flake8 (lint)

✅ Run Pytest (tests)

✅ Build Docker image

If everything passes → You’ll see a green ✅ in the GitHub Actions tab.

✅ Expected Output
🖥️ Local → App runs at http://127.0.0.1:8000/docs with Swagger UI

🤖 CI → Green ✅ if tests + lint + Docker build succeed

🐳 Docker → Runs containerized FastAPI app

📌 Notes for Beginners
📖 Swagger UI (/docs) → Interactive API playground (try requests).

📝 ReDoc (/redoc) → Clean documentation view.

🧪 Pytest ensures app works correctly.

✨ Flake8 enforces clean Python code.

🐳 Docker makes the app portable.

🤖 GitHub Actions automates everything on push.

🎯 Next Steps (Learning Roadmap)
🔹 Day 2 → Add CD with DockerHub (push images automatically)

🔹 Day 3 → Deploy on Kubernetes / Minikube

🔹 Day 4 → Add monitoring with Prometheus + Grafana

🔹 Day 5 → Setup full CI/CD pipeline

✨ Congratulations! You now have a working FastAPI + Docker + CI pipeline starter project 🎉
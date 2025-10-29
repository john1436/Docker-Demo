# 🐳 Python Docker Demo — Step-by-Step Guide (for EC2)

This project shows how to **run a simple Python app inside Docker**

---


**Dockerfile**
```dockerfile
FROM python:3.10-slim
WORKDIR /app
COPY . .
CMD ["python", "app.py"]

---


**app.py**
```app.py

print("Hello from Docker running inside an EC2 instance!")

---


## 🚀 How to Build and Run

```bash
# Build the Docker image
docker build -t py-demo .

# Run the container
docker run py-demo




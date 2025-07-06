# Guess-the-Capital
# 🌍 Guess the Capital – IBM Cloud Deployment

A simple web-based quiz game that asks users to guess the capital city of a country from four options. This project demonstrates how to containerize a front-end application and deploy it to the cloud using **Docker** and **IBM Cloud Code Engine**.

---

## 🚀 Project Objectives

1. Clone the source code
2. Build a Docker image
3. Deploy and test locally
4. Push image to IBM Cloud Container Registry
5. Deploy to IBM Cloud Code Engine

---

## 🧱 Technologies Used

- HTML, CSS, JavaScript
- Docker
- IBM Cloud
- IBM Cloud Code Engine
- IBM Cloud Container Registry

---

# Guess-the-Capital
# 🌍 Guess the Capital – IBM Cloud Deployment

A simple web-based quiz game that asks users to guess the capital city of a country from four options. This project demonstrates how to containerize a front-end application and deploy it to the cloud using **Docker** and **IBM Cloud Code Engine**.

---

## 🚀 Project Objectives

1. Clone the source code
2. Build a Docker image
3. Deploy and test locally
4. Push image to IBM Cloud Container Registry
5. Deploy to IBM Cloud Code Engine

---

## 🧱 Technologies Used

- HTML, CSS, JavaScript
- Docker
- IBM Cloud
- IBM Cloud Code Engine
- IBM Cloud Container Registry

---

## Guess-the-Capital
# 🌍 Guess the Capital – IBM Cloud Deployment

A simple web-based quiz game that asks users to guess the capital city of a country from four options. This project demonstrates how to containerize a front-end application and deploy it to the cloud using **Docker** and **IBM Cloud Code Engine**.

---

## 🚀 Project Objectives

1. Clone the source code
2. Build a Docker image
3. Deploy and test locally
4. Push image to IBM Cloud Container Registry
5. Deploy to IBM Cloud Code Engine

---

## 🧱 Technologies Used

- HTML, CSS, JavaScript
- Docker
- IBM Cloud
- IBM Cloud Code Engine
- IBM Cloud Container Registry

---
## 🐳 Local Setup with Docker

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ibm-developer-skills-network/fyidw-guess-the-capital.git
   cd fyidw-guess-the-capital

Build the Docker image:

bash
Copier
Modifier
docker build -t guess-the-capital 

Run the Docker container:

bash
Copier
Modifier
docker run -d -p 8080:80 guess-the-capital


☁️ Deploy to IBM Cloud Code Engine
Step 1: Build and Tag the Image
bash
Copier
Modifier
docker build -t us.icr.io/<your_namespace>/guess-the-capital .


Step 2: Push to IBM Container Registry
bash
Copier
Modifier
docker push us.icr.io/<your_namespace>/guess-the-capital

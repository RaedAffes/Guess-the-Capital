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

* HTML, CSS, JavaScript
* Docker
* IBM Cloud
* IBM Cloud Code Engine
* IBM Cloud Container Registry

---

## 📁 Project Structure

```bash
fyidw-guess-the-capital/
├── index.html        # Main HTML page
├── script.js         # Client-side JavaScript logic
├── style.css         # CSS styling
├── favicon.ico       # Favicon image
├── data.json         # Quiz data: countries and capitals
└── Dockerfile        # Docker instructions
```

---

## 🐳 Local Setup with Docker
 
1. **Clone the repository:**

   ```bash
   git clone https://github.com/<your-org>/fyidw-guess-the-capital.git
   cd fyidw-guess-the-capital
   ```

2. **Build the Docker image:**

   ```bash
   docker build -t guess-the-capital .
   ```

3. **Run the Docker container:**

   ```bash
   docker run -d -p 8080:80 guess-the-capital
   ```

4. **Access the application:**
   Open your browser and go to:
   `http://localhost:8080`

---

## ☁️ Deploy to IBM Cloud Code Engine

### Step 1: Build and Tag the Image

```bash
docker build -t us.icr.io/<your_namespace>/guess-the-capital .
```

### Step 2: Push to IBM Container Registry

```bash
docker push us.icr.io/<your_namespace>/guess-the-capital
```

### Step 3: Deploy with Code Engine 

```bash
ibmcloud ce application create \
  --name guess-the-capital \
  --image us.icr.io/<your_namespace>/guess-the-capital \
  --registry-secret icr-secret \
  --port 80
```

### Step 4: Get the Public URL

```bash
ibmcloud ce application get --name guess-the-capital
```

This will output a public URL like:

```
https://guess-the-capital-xyz123.us-south.codeengine.appdomain.cloud
```

---

## ✅ Example Live URL

> *Replace with your actual link once deployed:*

```text
https://guess-the-capital-xyz123.us-south.codeengine.appdomain.cloud
```



**Muhammad Yahya**
[LinkedIn](https://www.linkedin.com/in/1muhammadyahya/)

---

© IBM Corporation. All rights reserved.

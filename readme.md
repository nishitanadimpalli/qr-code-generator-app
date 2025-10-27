# QR Code Generator (Dockerized)

This is a simple **QR Code Generator** application written in Python and containerized using Docker.  
It takes a URL as input and creates a QR code image saved in the `qr_codes` folder.

---

## 🛠 How to Run

### 1. Build Docker Image
```bash
docker build -t qr-code-generator-app .

Run Container
docker run -d --name qr-generator qr-code-generator-app

Check Logs
docker logs qr-generator

Stop and Remove Container
docker stop qr-generator
docker rm qr-generator

Run with Custom URL

You can pass a different URL:

docker run --rm qr-code-generator-app --url https://www.njit.edu

Push to Docker Hub
docker login
docker tag qr-code-generator-app yourusername/qr-code-generator-app
docker push yourusername/qr-code-generator-app

# Reflection: Dockerizing the QR Code Generator

**What I Did:**  
Installed Docker Desktop with WSL2, built and ran a secure QR Code Generator container, created a slim Dockerfile with a non-root user, pushed the image to DockerHub, and automated builds with GitHub Actions.

**Challenges:**  
Email verification blocking DockerHub push, mapping volume correctly, and understanding the difference between ENTRYPOINT and CMD.

**Security Considerations:**  
Used a non-root user, lightweight python:3.12-slim image, and `.dockerignore` to exclude unnecessary files.

**What I Learned:**  
- Docker image layering and caching  
- Volume mounting between container and host  
- Overriding CMD arguments at runtime  
- Continuous Integration using GitHub Actions

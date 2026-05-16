# Kubernetes Phishing Project

## Overview
This project is a Kubernetes-based web application that simulates a login system. It includes a frontend, backend API, and MySQL database, all deployed and managed using Kubernetes manifests.

The system demonstrates how microservices communicate inside a Kubernetes cluster using Services and Ingress.

## Architecture
The project consists of the following components:

- Frontend Service → Handles user interface (login page)
- Backend Service → Processes login requests 
- MySQL Database → Stores application data
- Ingress Controller → Routes external traffic to services
- Persistent Storage (PV & PVC) → Ensures database data persistence

## Technologies Used
- Kubernetes
- Docker
- MySQL 8.0
- Nginx Ingress Controller
- YAML

## Project Structure
k8s-project/
│
├── frontend.yaml
├── backend.yaml
├── mysql.yaml
├── frontend-service.yaml
├── backend-service.yaml
├── mysql-service.yaml
├── ingress.yaml
├── pv.yaml
├── pvc.yaml

## How It Works

1. User opens:
   http://phishing.local

2. Frontend loads login page

3. Login request sent to:
   POST /submit

4. Request is routed through Kubernetes Ingress to backend service

5. Backend processes request and interacts with MySQL database

## Features Demonstrated

- Microservices architecture using Kubernetes
- Kubernetes Deployments & Services
- Ingress routing
- Persistent storage (PV/PVC)
- Backend–database communication
- Frontend–backend integration

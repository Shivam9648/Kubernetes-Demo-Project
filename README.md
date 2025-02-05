# Kubernetes-Demo-Project

# 📌 Overview
  This project is a Kubernetes Demo created for studying the core features of Kubernetes, including:

 * Self-healing mechanisms
 * Scaling multiple pods
 * YAML configuration
 * Deployments and Services
 * Using Docker images in Kubernetes
 The project was built using Kubernetes official documentation as a reference.

# 🚀 Features

 * Deployment Configuration: Defines how the application runs in Kubernetes, including replica count, container image, and restart policies.
 * Service Configuration: Exposes the application to the network and manages communication between pods.
 * Self-healing: Kubernetes automatically restarts failed containers.
 * Scaling: The number of pods can be increased or decreased based on requirements.
 * Dockerized Application: The app is containerized using Docker and deployed in Kubernetes.

 # 📂 Project Structure
   /kubernetes-demo
 │── deployment.yaml  # Kubernetes Deployment configuration
 │── service.yaml     # Kubernetes Service configuration
 │── Dockerfile       # Dockerfile for building the container
 │── app/             # Application source code
 │── README.md        # Project documentation

# 🛠️ How to Run
1. Clone the repository
 
   git clone https://github.com/your-username/kubernetes-demo.git
   cd kubernetes-demo

3. Build and push the Docker image
 
   docker build -t your-dockerhub-username/kubernetes-demo .
   docker push your-dockerhub-username/kubernetes-demo

5. Apply Kubernetes configurations

   kubectl apply -f deployment.yaml
   kubectl apply -f service.yaml

7. Check running pods and services

   kubectl get pods
   kubectl get services

9. Scale the application (Example: 3 replicas)
    
   kubectl scale deployment kubernetes-demo --replicas=3

11. Test the application using Minikube
    
    minikube service kubernetes-demo

# 📖 Learning Outcomes
   * Kubernetes Deployment and Service Configurations
   * Self-healing and container restarts
   * Scaling pods dynamically
   * Containerizing applications using Docker
   * Applying YAML configurations in Kubernetes

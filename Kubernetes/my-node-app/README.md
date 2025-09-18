# My Node.js Application

This is a simple Node.js application that demonstrates how to containerize a Node.js app using Docker and deploy it on Kubernetes.

## Prerequisites

- Node.js and npm installed on your machine.
- Docker installed on your machine.
- Kubernetes cluster (e.g., Minikube, GKE, EKS) set up and configured.

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/microsoft/vscode-remote-try-node.git
cd my-node-app
```

### Install Dependencies

Run the following command to install the necessary dependencies:

```bash
npm install
```

### Build the Docker Image

To build the Docker image for the application, run:

```bash
docker build -t my-node-app .
```

### Run the Application Locally

You can run the application locally using the following command:

```bash
node src/index.js
```

The application will be available at `http://localhost:3000`.

### Deploying to Kubernetes

1. **Create the Deployment:**

   Apply the deployment configuration:

   ```bash
   kubectl apply -f kubernetes/deployment.yaml
   ```

2. **Create the Service:**

   Apply the service configuration:

   ```bash
   kubectl apply -f kubernetes/service.yaml
   ```

3. **Access the Application:**

   Depending on your service type, you can access the application using the appropriate method (e.g., `kubectl port-forward` for ClusterIP services).

## License

This project is licensed under the MIT License. See the LICENSE file for details.
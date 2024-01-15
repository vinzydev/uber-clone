
---

# AutomateHub: CI/CD Blueprint for RideShare Replica with Proactive Monitoring Implementation

## Introduction:
Embark on a transformative journey with "Jenkins Driven: CI/CD for Uber Clone with Monitoring Excellence" — an instructive guide that reveals the seamless creation of an Uber-like application. 🚀 Leveraging the power of Jenkins, this manual guides you through the utilization of Amazon’s resources, configuring components with Terraform, and orchestrating with Docker and Kubernetes. The surveillance aspect is enhanced by integrating Grafana and Prometheus to vigilantly monitor your application. 🌐

This comprehensive, step-by-step guide ensures the safety and optimal performance of your Amazon-style app, guiding you from code inception to live deployment. 🛠️💻 Come aboard, and together, let’s craft your very own Uber Clone!

## Technologies Used in This Project:
In the realm of Uber Clone development, a robust DevOps ecosystem plays a pivotal role in streamlining processes and ensuring optimal performance. Let’s explore the key components that contribute to the seamless integration and continuous delivery of your Uber Clone application.

- **Jenkins:** Automating Your Workflow
- **Terraform:** The Infrastructure Magician
- **Docker:** Containerization Excellence
- **Kubernetes:** The Deployment Maestro
- **Grafana:** Visualize, Monitor, Excel
- **Prometheus:** Your Vigilant Guardian

In synergy, Jenkins, Terraform, Docker, Kubernetes, Grafana, and Prometheus form a powerful DevOps ensemble, elevating your Uber Clone development to new heights of efficiency and reliability.

## Project Overview:
**GitHub Repository:** [https://github.com/mudit097/uber-clone](https://github.com/mudit097/uber-clone)

**Blog:** [AutomateHub: CI/CD Blueprint for RideShare Replica with Proactive Monitoring Implementation](https://muditmathur121.medium.com/automatehub-ci-cd-blueprint-for-rideshare-replica-with-proactive-monitoring-implementation-e4e97a3fa834)

**Video:** [Watch the Video](https://drive.google.com/file/d/1yRPmPAkL37_JgI9RiXdHj_Wq89JuHrL3/view?usp=sharing)

### Step 1: Launch an Ubuntu instance (T2.large)
1. Sign in to AWS Console.
2. Navigate to EC2 Dashboard.
3. Launch an instance with Ubuntu AMI, T2.large type, and appropriate configurations.
4. Configure security groups and key pairs.
5. Access the EC2 instance using the key pair and public IP/DNS.

### Step 2: Create IAM role
1. Navigate to IAM in the AWS console.
2. Create a new IAM role for EC2 with Administrator Access.
3. Attach the created role to the EC2 instance for cluster provisioning.

### Step 3: Installations of Packages
1. Run script1.sh for Jenkins, Docker, and other package installations.
2. Run script2.sh for Trivy, Terraform, kubectl, AWS CLI, and Helm installations.

### Step 4: Connect to Jenkins and Sonarqube
1. Access Jenkins on `<EC2-ip:8080>`, set up Jenkins, and install recommended plugins.
2. Access Sonarqube on `<EC2-ip:9000>`, create a token, and integrate with Jenkins.

### Steps 5-9: Terraform plugin install, EKS provision, Pipeline Setup, Plugins Installation, Configure in Global Tool Configuration, and Docker Setup
1. Install Terraform plugin in Jenkins.
2. Modify the S3 bucket name in the backend.tf file.
3. Create a pipeline job for EKS provisioning with build parameters.
4. Setup Jenkins pipeline with stages for Git, Sonarqube, Quality Gate, Install Dependencies, and Docker.
5. Install required plugins in Jenkins.
6. Configure global tools for Java, Sonar, Nodejs, OWASP, and Docker.
7. Configure Sonar Server in Manage Jenkins with Sonar token.

### Step 10: Kubernetes Deployment
1. Configure AWS CLI on Jenkins instance.
2. Update Kubeconfig with EKS cluster information.
3. Create a pipeline stage for deploying to Kubernetes.

### Step 11: Setup Monitoring on cluster
1. Create a new pipeline for setting up Helm repositories and deploying Prometheus.
2. Patch Prometheus and Grafana services for LoadBalancer.
3. Get service URLs for Prometheus and Grafana.

### Step 12: Destroy EKS cluster when done with the project
1. Create a pipeline for destroying EKS cluster using Helm.

## Conclusion
Building an app like Uber with Jenkins has been exciting! 🚀 Jenkins helps smoothly put together Uber’s virtual world, like arranging blocks. It makes sure everything works well, and we’ve added special guards, Grafana and Prometheus, to watch over the app. 🌐 This guide takes you through each step, making sure your Uber Clone is safe and works great, from writing code to making it live. 🛠️💻 Let’s celebrate this success and make your Uber Clone even better!

# Netflix Stack Bootcamp Assignment - DevOps BootCamp 2024

## Overview
This project is the final submission for the Netflix Stack Bootcamp, showcasing a microservices architecture deployed on AWS EC2 instances. The stack includes multiple services such as Nginx for load balancing and reverse proxy, a Node.js-based NetflixFrontend, and a Flask-based NetflixMovieCatalog API.

## Objectives
- **Nginx**: Acts as a reverse proxy and load balancer.
- **NetflixFrontend**: Node.js-based web application serving as the user interface for Netflix-like movie browsing.
- **NetflixMovieCatalog**: Flask API serving movie data for the frontend.

## Key Features
- **Microservices Architecture**: Each service is containerized using Docker and deployed on separate EC2 instances.
- **CI/CD Pipelines**: Implemented using GitHub Actions for continuous integration and deployment.
  - NetflixFrontend (Node.js)
  - NetflixMovieCatalog (Flask API)
  - Nginx configuration updates.
- **Infrastructure as Code (IaC)**: Terraform was used for provisioning EC2 instances and other infrastructure components.
- **High Availability**: Nginx configured as a load balancer to manage multiple instances of NetflixFrontend for high availability.
- **AWS Route 53**: A registered domain to access the application services.

## Deployed Application
- **Live Demo**: [Netflix Stack Application](http://netflix.devops-days-upes.com/) 
## Repositories
- [NetflixMovieCatalog](https://github.com/Jahnavi-Anand/NetflixMovieCatalog.git) - Flask-based API.
- [NetflixFrontend](https://github.com/Jahnavi-Anand/NetflixFrontend.git) - Node.js frontend application.

## DevOps Practices
1. **Docker Containers**: All services (Nginx, NetflixFrontend, NetflixMovieCatalog) are containerized.
2. **CI/CD Pipelines**: Automated build and deploy pipelines using GitHub Actions.
3. **Nginx Load Balancer**: Configured to distribute traffic among multiple NetflixFrontend instances.
4. **AWS Infrastructure**: EC2 instances provisioned via Terraform for scalable and automated deployment.

## Technologies Used
- **AWS**: EC2, Route 53
- **Nginx**: HTTP engine, reverse proxy, load balancer
- **Docker**: Containerization of all services
- **GitHub Actions**: CI/CD pipeline for build and deployment automation
- **Terraform**: Infrastructure provisioning
- **Flask**: Backend API (NetflixMovieCatalog)
- **Node.js**: Frontend web application (NetflixFrontend)

## How to Run Locally
1. Clone both repositories:
   - `git clone https://github.com/Jahnavi-Anand/NetflixMovieCatalog.git`
   - `git clone https://github.com/Jahnavi-Anand/NetflixFrontend.git`
2. Use Docker Compose to spin up containers for the services.
3. Visit the frontend on `localhost:3000` once services are up.

## Conclusion
This project showcases a fully deployed microservices architecture using best DevOps practices such as Docker, CI/CD, IaC, and high availability architecture.

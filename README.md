# DevOps Syllabus

## COURSE OUTLINE

### Introduction  								15 Min
- Course Features and Tools
- What is DevOps?
- A brief overview of the history of DevOps

### DevOps Culture								15 Min
- The Goals of DevOps
- DevOps vs Traditional Silos

### DevOps Concepts and Practises				45 Min
- Build Automation
- Continuous Integration
- Continuous Delivery and Continuous Deployment
- Infrastructure as Code
- Configuration Management
- Container Orchestration
- Monitoring
- Microservices

### DevOps Tools 								45 Min
- Introduction to DevOps Tools
- Tools for Build Automation and Continuous Integration
- Tools for Configuration Management
- Tools for Virtualization and Containerization
- Tools for Monitoring
- Tools for Orchestration

# Source Code Management
## Git Basics

### The Basics of Using Git					1 Hr 30 Min
- Understanding the Git Filesystem
- Creating a Local Repository (Empty)
- Basic Configuration of Git
- Adding Files to Project
- The Status of your project
- Commiting to Git
- Ignoring Certain File Types
- HOL: Creating Local Repositories with Git and Adding/Checking in Files

### Tags, Branching, Merging and Reverting 	45 Min
- Using Tags
- Using Branches
- Merging Branches
- Rebasing
- Reverting a Commit
- Using the 'diff' Command

### Git's Logs and Auditing					15 Min
- Using Git's Logs

### Cloning Repositories 					1 Hr
- Cloning Local Repositories
- Cloning Remote Repositories over HTTPS, SSH
- Forking
- HOL: Securing Your Github Account with SSH Keys
- HOL: Cloning a Remote GitHub Repository

### Push, Pull, and Tracking Remote Repositories 	30 Min
- Tracking Remote Repositories
- Pushing to Remote Repositories
- Pull Requests

### Git Branching Strategy							30 Min
- What is a branching strategy?
- Why you need a branching strategy
- What are some common Git branching strategies?
	- GitFlow
	- GitHub Flow
	- GitLab Flow
	- Trunk-based Development

# Build Automation and Continuous Integration
## Build Automation									2 Hr
- Introducing Build Automation
- Build Automation Tools
	- gradle
	- npm
	- make
	- Packer

- HOL: Creating Build Automation with Gradle
- HOL: Automate AMI image creation with Packer

## Continuous Integration & Jenkins Pipelines		3 Hr
- CI Overview
- Installing Jenkins
- Scripted vs. Declarative Pipelines
	- Scripted Pipelines
	- Declarative Pipelines
	- Groovy and DSL
- Jenkinsfile Basics
- Upstream, Downstream, and Triggers
	- Artifacts and Fingerprints
	- Linking Jobs
	- Automating Jobs
	- HOL: Linking Jobs in Jenkins
	- HOL: Building multibranch build job with dependency between multiple job
- FreeStyle Jobs
	- Basic Job Structure
	- Parameters
	- Notifications
	- HOL: Building a Freestyle Job in Jenkins
- Agents and Distributed Builds
	- Setting up a Build Agent
	- Distributing  a Build
	- HOL: Distributing a Jenkins Build
Jenkins on the Command Line
	- Using the Jenkins API
	- Using the Jenkins CLI

## Continuous Delivery and Continuous Deployment					3 Hr
- What is Continuous Delivery and Continuous Deployment
- Continous Delivery vs. Continuous Deployment
- Bringing CI and CD (and CD) Together
- Continuous Delivery Release Automation
	- Automated Deployment
	- Configuration Management
- HOL: Implementing Automated Deployment Through a Jenkins Pipeline
- HOL: Provide Continuous Delivery with GitHub and Terraform Cloud for AWS

# Infrastructure Automation
## DevOps Tools for Infrastructure Automation		30 Min
- Infrastructure Provisioning
- Configuration Management
- Continuous Integration/Deployment
- Config/Secret Management
- Logging and Monitoring

## Understanding Infrastructure as a code				30 Min
- IaC and Its Benefits
- Cloud Agnostic IaC with Terraform

## IaC with Terraform									6 Hr
- What is the Terraform Workflow?
- Terraform Key Concepts: Plan, Apply, and Destroy
- Resource Addressing in Terrafrom: Understanding Terraform Code
- Terraform Fundamentals
	- Terraform State
	- Terraform Variables and Outputs
	- Terraform Provisioners
- HOL: Deploying a VM in AWS Using the Terraform Workflow
- HOL: Using Terraform Provisioner to Setup an Nginx Proxy on AWS
- Terraform Modules
	- Accessing and Using Terraform Modules
	- Interacting with Terraform Module Inputs and Outputs
- HOL: Building and Testing a Basic Terraform Module
- Built-in Funtions and Dynamics Blocks
	- Terraform Built-in Functions
	- Terraform Dynamic Blocks
- HOL: Using Terraform Dynamic Blocks and Built-in Functions to Deploy to AWS

## Configuration Management with Ansible				6 Hr
- What is Configuration Management?
- What is Ansible?
- Installation and Configuration
	- HOL: Deploying Ansible
	- HOL: Getting Started with Ansible
	- HOL: Ad-Hoc Ansible Commands
	- HOL: Working with Ansible Inventories
- Ansible Tasks
- Plays and Playbooks
	- HOL: Ansible Playbooks: The Basics
	- HOL: Working with Ansible Templates, Variables, and Facts
	- HOL: Deploying Services Using Ansible
	- HOL: Advanced Features in Ansible Playbooks
- Roles
	- HOL: Working with Ansible Roles
- Ansible Vault
	- HOL: Working with Confedential Data in Ansible
- Building Playbooks for Jenkins Master Setup
- Building Playbooks for Jenkins Worker Setup
- Building Jinja2 Templates for Ansible Playbooks


# Containers and Orchestration

## Docker Community Edition Installation and Configuration   2 Hr
- Intalling Docker Community Edition
- Docker Basics
	- Docker Commands
	- Creating Containers
	- Exposing Container Ports
	- Executing Container Commands
	- Docker Logging
- Networking
- Storage and Volumes
- Selecting a Storage Driver
- Running a Container
- Namespaces and Cgroups
- HOL: Installing and Configuring the Docker Engine

## Image Creation, Management, and Registry       3 Hr
- Introduction to Docker Images
- The Compoments of a Dockerfile
- More Dockerfile Directives
- Building Efficient Images
- Managing Images
- Flattening a Docker Image to a Single Layer
- Introduction to Docker Registries
- Using Docker Registries
- HOL: Creating Your Own Docker Image
- HOL: Building a Private Docker Registry
- HOL: Building Crosplatform Images Using Multi-Stage Build

## Docker Compose 								2 Hr
- Introduction to Docker Service
- Compose Commands
- Creating a Compose File
- Using Volumes and Networking with Compose
- HOL: Building a Microservices with Docker Compose


## Kubernetes - Container Orchestrator						10 Hr
- Kubernetes Fundamentals
	- Kubernetes Fundamentals Intro
	- Exploring Kubernetes Architecture
	- Kubernetes Objects
- Kubernetes Networking
- Kubernetes Networking Basics
- Kubernetes Service Fundamentals
- Service Types
- Kubernetes Storage
	- Kubernetes Storage Big Picture
	- Persistent Volumes and Persistent Volume Claims
	- Storage Clases
- Kubernetes Deployments
- Scaling Applications Automatically
	- Horizontal Pod Autoscaler
	- Cluster Autoscaler
- RBAC and Admission Control
- HOL: Working with Kubernetes Namespace
- HOL: Managing Kubernetes Applications With Deployments
- HOL: Exposing Kubernetes Pods Using Services
- HOL: Using Kubernetes Services with DNS
- HOL: Using Kubernetes Ingress
- HOL: Managing Container Storage With Kubernetes Volumes
- HOL: Using PersistentVolumes in Kubernetes
- Troubleshooting
	- Kubernetes Troubleshooting Overview
	- Checking Cluster and Node Logs
	- Checking Containers Logs
	- Troubleshooting Kubernetes Networkign Issues
- HOL: Troubleshooting a Broken Kubernetes Cluster
- HOL: Troubleshooting a Broker Kubernetes Application

# Monitoring and Logging
## Monitoring with Prometheous and Graphana			7 Hr
- Monitoring Basics
	- Push or Pull
	- Service Discovery
	- HOL: Setting Up Prometheous and Adding Endpoints
- Infrastructure Monitoring
	- Using the Node Exporter
	- CPU Metrics
	- Memory Metrics
	- Disk Metrics
	- File System Metrics
	- Networking Metrics
	- Load Metrics
	- Using cAdvisor to Monitor Containers
	- HOL: Monitoring Infrastructure and Containers with Prometheous
- Application Monitoring
	- Using a Client Library
	- Counters
	- Gauges
	- Summeries and Histograms
	- HOL: Application Monitoring with Prometheous
- Manageing Alerts
	- Recording Rules
	- Alerting Rules
	- Using Alertmanager
	- Silences
	- HOL: Using Alertmanager with Prometheous
- Visualization
	- Adding a Dashboard
	- Building a Panel
	- HOL: Using Grafana to Visualize Prometheous Data


### DevOps and the Cloud 						8 Hr
- DevOps and the Cloud
- DevOps and Google Cloud Platform
	- HOL: Running Microservice in GKS using Helm
- DevOps and Microsoft Azure
- DevOps and Amazon Web Services
	- AWS Services
	- Identity and Access Management (IAM)
	- Serverless Architecture
		- Computing with Lambda
		- Running Containers in ECS
	- Application Monitoring with CloudWatch
	- Elastic Load Balancing(ELB)
		- Using Application Load Balancers
	- High Availability and Scaling
		- Ec2 Instance Auto Scaling
	- HOL: Triggering AWS Lambda from Amazon SQS
	- HOL: Create and Assume Roles in AWS
	- HOL: User Application Load Balancers for Web Servers
	- HOL: Implement Advanced CloudWatch Monitoring for a Web Server
	- HOL: Work with AWS VPC Flow Logs for Network Monitoring

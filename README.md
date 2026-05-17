# Self-Healing DevOps Deployment Platform

A cloud-native DevOps automation platform designed to demonstrate CI/CD automation, Kubernetes self-healing capabilities, infrastructure monitoring, and container orchestration using Jenkins, Docker, Kubernetes, Prometheus, and Grafana.

---

# Project Overview

This project automates the software deployment lifecycle using Jenkins pipelines and Kubernetes orchestration.

The platform is capable of:

- Automating Docker image build and deployment
- Deploying applications into Kubernetes clusters
- Performing self-healing recovery using Kubernetes probes
- Monitoring infrastructure and container health
- Visualizing metrics using Grafana dashboards
- Simulating failure recovery scenarios

---

# Architecture

```text
Developer Push
       ↓
    GitHub
       ↓
    Jenkins Pipeline
       ↓
 Docker Image Build
       ↓
   DockerHub
       ↓

```

# Ansible Automation

This directory contains Ansible playbooks used for infrastructure automation and server configuration.

## Current Automation Tasks

- Docker installation
- Service management
- Package updates
- Infrastructure configuration

## Future Improvements

- Jenkins installation automation
- Kubernetes node setup
- Tomcat deployment automation
- Monitoring agent installation
 Kubernetes Cluster
       ↓
Self-Healing Recovery
       ↓
Prometheus + Grafana

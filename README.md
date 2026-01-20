# Highly Available Web Application Deployment on AWS EKS

## Overview
This project demonstrates deployment of a highly available web application on AWS EKS using Kubernetes. The application is resilient, scalable, and persistent.

## Problem
Single-server applications suffer downtime and data loss. This project solves these problems with Kubernetes and AWS services.

## Solution
- Multi-pod deployment for high availability
- LoadBalancer for public access
- Persistent Volume for durable storage
- Auto-healing pods

## Architecture
- Amazon EKS Cluster
- EC2 Worker Nodes
- Kubernetes Deployment, Service, PVC
- Nginx container for website hosting
- AWS EBS Persistent Volume for storage

## Key Features
- High Availability
- Auto Healing
- Zero Downtime
- Persistent Storage
- Cloud-Native Deployment

## File Structure
- kubernetes/ → Deployment, Service, PVC
- website/ → HTML and images
- architecture/ → Architecture diagram


## Tools Used
AWS EKS, Kubernetes, Docker, Nginx, AWS EBS, kubectl, eksctl, HTML/CSS

## Deployment Steps
1. Create EKS cluster
2. Deploy application using deployment.yaml
3. Expose using service.yaml (LoadBalancer)
4. Attach PVC using pvc.yaml
5. Upload website files to pod

## Demo
- Delete pod → new pod auto-created
- Website persists → PVC works

## Website

The static website is hosted in `website/` folder with all images in `website/images/`.

## Live Demo 
http://aeb4f0f256d054d32b78017362ddfaeb-1887267208.ap-south-1.elb.amazonaws.com/

## Conclusion
This repo contains all files to create a highly available, persistent web application on AWS EKS.


# AWS Cloud Resume Challenge

Status: In Progress

This repository holds the static resume site for the [Cloud Resume Challenge](https://cloudresumechallenge.dev/), a hands-on project used to demonstrate practical AWS, networking, and infrastructure skills by building and hosting a personal resume entirely on AWS.

## Overview

The site is a plain HTML/CSS resume (`index.html` and `styles.css`) designed to be hosted as a static website through Amazon S3 and served securely and globally through Amazon Route 53. The project is being built around a 3-tier VPC architecture, with a focus on secure networking, least-privilege access, and operational visibility.

## Planned architecture

- **Static hosting:** Amazon S3 bucket configured for static website hosting
- **DNS and delivery:** Amazon Route 53 for domain routing
- **Networking:** Custom VPC with public and private subnets, a NAT gateway for outbound traffic from private resources, and Network ACLs for subnet-level traffic control
- **Access control:** Security Groups scoped to only the traffic each resource actually needs
- **Identity and access management:** Least-privilege IAM policies and roles, avoiding broad or wildcard permissions
- **Monitoring:** Amazon CloudWatch for metrics, logs, and alarms on the deployed infrastructure

## Repository contents

- `index.html`: the resume content, structured with semantic HTML
- `styles.css`: styling for the resume, formatted to resemble a traditional single-page resume
- `README.md`: this file

## Goals

- Deploy the resume as a live, publicly accessible static website
- Apply infrastructure and networking concepts from coursework and certifications (AWS Cloud Practitioner, Network+) in a real, working environment
- Practice least-privilege security design from the start rather than adding restrictions later
- Build a foundation that can later be extended with a visitor counter, CI/CD pipeline, and infrastructure as code, in line with the broader Cloud Resume Challenge scope

## Status notes

This project is actively in progress. The resume content and styling are complete. The AWS infrastructure (VPC, subnets, S3 hosting, Route 53, IAM policies, and CloudWatch monitoring) is currently being built out. This README will be updated as each piece of the architecture is deployed.

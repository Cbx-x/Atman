# Atman: Autonomous Reconnaissance and Intelligence Platform

An intelligent cybersecurity platform for automated asset discovery, reconnaissance, vulnerability detection, and real-time security intelligence.

## Overview

Atman is a centralized reconnaissance and vulnerability management platform designed to help security teams, researchers, and organizations continuously monitor their external attack surface.

The platform automates asset discovery, subdomain enumeration, endpoint identification, service fingerprinting, vulnerability scanning, and reporting through a unified dashboard.

## Key Features

* Automated asset discovery
* Subdomain enumeration and monitoring
* Port scanning and service fingerprinting
* Vulnerability detection and classification
* OSINT data collection
* Real-time scan progress updates
* Severity-based vulnerability prioritization
* Interactive security dashboard
* Historical scan tracking
* Role-Based Access Control (RBAC)
* Report generation (PDF and CSV)

## System Architecture

<img width="600" height="600" alt="image" src="https://github.com/user-attachments/assets/efa738a9-dc89-4389-b817-e05aeeb00c7e" />


## Technology Stack

### Backend

* Python 3.10+
* Django
* Django REST Framework (DRF)
* Celery
* Redis
* PostgreSQL
* Django Channels

### Frontend

* Next.js
* React
* Tailwind CSS
* ShadCN/UI
* Redux Toolkit
* Axios
* SWR
* Recharts

### Infrastructure

* Docker
* Docker Compose
* Nginx
* AWS / DigitalOcean / Hetzner

## Architecture Workflow

1. User initiates a reconnaissance scan.
2. Backend validates requests and schedules tasks.
3. Celery workers execute reconnaissance modules asynchronously.
4. Redis manages task queues and messaging.
5. Reconnaissance modules perform asset discovery and vulnerability assessment.
6. Results are stored in PostgreSQL.
7. Dashboard displays real-time intelligence and reports.

## Reconnaissance Modules

* Asset Discovery
* Subdomain Enumeration
* Port Scanning
* Service Fingerprinting
* Vulnerability Detection
* OSINT Collection

## Dashboard

<img width="600" height="300" alt="WhatsApp Image 2025-12-20 at 12 19 09 PM (2)" src="https://github.com/user-attachments/assets/d1140e36-16a1-4916-b88d-2413de3bb3fb" />

The dashboard provides:

* Total targets
* Discovered subdomains
* Active endpoints
* Vulnerability statistics
* Scan activity feed
* Geographic asset distribution

## How It Works

### Step 1: Add Target

<img width="600" height="300" alt="WhatsApp Image 2025-12-20 at 12 19 03 PM" src="https://github.com/user-attachments/assets/6df48028-3c11-4a46-9807-3269661d1de0" />



Provide a domain name, IP address, CIDR range, or URL.

### Step 2: Select Scan Type

<img width="600" height="300" alt="WhatsApp Image 2025-12-20 at 12 19 01 PM" src="https://github.com/user-attachments/assets/d185547d-7dd3-4039-ab7f-7a636bef0d74" />


Available scan options:

* Atman Recommended Scan
* Subdomain Scan
* Port Scan
* OSINT Scan
* Vulnerability Scan
* Full Scan

The platform performs asynchronous reconnaissance and vulnerability assessment.

### Step 3: Execute Scan & Analyze Results

<img width="600" height="300" alt="WhatsApp Image 2025-12-20 at 12 19 03 PM (1)" src="https://github.com/user-attachments/assets/98a35c42-908e-49f3-ae50-62952915a359" />


View:

* Discovered assets
* Active services
* Vulnerabilities by severity
* Historical scan data

## Installation

### Prerequisites

* Docker
* Docker Compose
* Git

### Clone the Repository

```bash
git clone https://github.com/your-username/atman-security.git
cd atman-security
```

### Start the Application

```bash
docker-compose up --build
```

### Access the Platform

Frontend:

```text
http://localhost:3000
```

Backend API:

```text
http://localhost:8000
```

## Project Structure

```text
atman-security/
├── backend/
├── frontend/
├── docker/
├── docs/
├── screenshots/
├── nginx/
└── docker-compose.yml
```

## Future Enhancements

* AI-based vulnerability prioritization
* Automated remediation workflows
* Multi-cloud asset discovery
* Container and Kubernetes security
* Threat intelligence integration

## Acknowledgements

Developed as a Final Year Project at:

**Department of CSE (IoT & CSBT)**

SEA College of Engineering and Technology, Bengaluru

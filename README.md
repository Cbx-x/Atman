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

![Atman System Architecture](screenshots/system-architecture.png)

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

![Dashboard Overview](<img width="600" height="300" alt="WhatsApp Image 2025-12-20 at 12 19 09 PM (2)" src="https://github.com/user-attachments/assets/d1140e36-16a1-4916-b88d-2413de3bb3fb" />
)

The dashboard provides:

* Total targets
* Discovered subdomains
* Active endpoints
* Vulnerability statistics
* Scan activity feed
* Geographic asset distribution

## How It Works

### Step 1: Add Target

![Add Target](screenshots/add-target.png)

Provide a domain name, IP address, CIDR range, or URL.

### Step 2: Select Scan Type

![Select Scan Type](screenshots/select-scan.png)

Available scan options:

* Atman Recommended Scan
* Subdomain Scan
* Port Scan
* OSINT Scan
* Vulnerability Scan
* Full Scan

### Step 3: Execute Scan

![Scan Execution](screenshots/scan-execution.png)

The platform performs asynchronous reconnaissance and vulnerability assessment.

### Step 4: Analyze Results

![Vulnerability Overview](screenshots/vulnerability-overview.png)

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

## Team Members

* Member 1 – Project Lead / Backend Development
* Member 2 – Frontend Development
* Member 3 – Reconnaissance Modules & Security Testing
* Member 4 – DevOps, Documentation & Deployment

## Future Enhancements

* AI-based vulnerability prioritization
* Automated remediation workflows
* Multi-cloud asset discovery
* Container and Kubernetes security
* Threat intelligence integration

## License

This project is developed for academic and research purposes.

## Acknowledgements

Developed as a Final Year Project at:

**Department of CSE (IoT & CSBT)**

SEA College of Engineering and Technology, Bengaluru

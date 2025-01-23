# 🛡️ Implementation of an Anti-Virus Protection System

## 📖 Overview
This project involves the implementation of a comprehensive antivirus protection system, focusing on information security solutions. The following aspects will be addressed:

- Understanding the necessary data for determining the optimal deployment scenario.
- Familiarization with system requirements.
- Deployment of the solution and task formulation.

---

## 📑 Table of Contents
- [Project Goals](#-project-goals)
- [System Requirements](#-system-requirements)
- [Implementation Details](#-implementation-details)
- [Features](#-features)
- [Usage](#-usage)
- [Contributions](#-contributions)
- [License](#-license)

---

## 🎯 Project Goals
The goal of this project is to design and implement an antivirus protection system with the following key components:

1. **Management Servers**: Centralized control of antivirus protection.
2. **Workstation Protection Module**: Secure all workstations in the domain.
3. **Server Protection Module**: Secure all servers in the domain.

All assets will be part of an **Active Directory (AD)** domain, ensuring a unified and manageable infrastructure.

---

## 📋 System Requirements

### Hardware and Software Requirements:
- **Management Server**:
  - Operating System: Microsoft Windows Server.
  - Database Management: PostgreSQL for storing service information.
  - Active Directory domain integration.

- **Workstations and Servers**:
  - Antivirus software distributed centrally from the management server.

### Functional Requirements:
1. The management server must:
   - Scan specified network ranges and domains for new hosts.
   - Distribute antivirus software, modules, and databases centrally to assets based on their administrative group.
   - Update antivirus software and modules automatically on a schedule.
2. Workstations must:
   - Implement a policy to block selected categories of applications.
   - Send critical events to the management server.
3. Events from connected devices must:
   - Be logged in the event log of the management server.
   - Be sent to a SIEM system for monitoring information security events.
4. Remote technical support:
   - Technical specialists can view asset information and connect to a remote desktop without management rights.

---

## ⚙️ Implementation Details

### Deployment Steps:
1. **Pre-Project Survey**:
   - Conduct inventory and gather all necessary data about the infrastructure.
2. **Task Formulation**:
   - Define detailed requirements for the system to form the basis of the terms of reference.
3. **Design**:
   - Develop a technical solution describing the architecture and functioning of the system.
4. **Setup**:
   - Configure the management server, PostgreSQL database, and SIEM integration.
5. **Testing**:
   - Execute test programs to ensure the system meets functional requirements.
6. **Deployment**:
   - Roll out the solution across the infrastructure.

---

## ✨ Features
- Centralized antivirus management.
- Automatic updates for antivirus software and modules.
- Blocking policies for unauthorized applications.
- Event logging and SIEM integration for enhanced security monitoring.
- Remote support with view-only access.

---

## 🚀 Usage

### Installation:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/Implementation-of-an-anti-virus-protection-system.git
   ```
2. Configure the management server with PostgreSQL and connect it to the AD domain.
3. Deploy workstation and server protection modules.
4. Configure automatic updates and application-blocking policies.

### Running the System:
1. Start the management server services.
2. Monitor events and updates through the management dashboard.
3. Review critical events in the SIEM system for timely incident response.

---

## 🤝 Contributions
Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add your feature description"
   ```
4. Push to your forked repository and create a pull request.


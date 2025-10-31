# DevOps & CI/CD Notes

## Package Managers
- **mvn** – Maven (Java)
- **npm** – Node.js
- **pip** – Python

## Build & Testing
- **Build** – Compiles the code, but **does not run unit tests**  
- **`mvn package` / `mvn install`** – Compiles the code **and runs unit tests**

## Continuous Integration (CI)
Triggered on:
- Merging a PR
- Merging to a branch
- Pushing to the codebase

**CI Pipeline:**
1. Code Checkout
2. Linting
3. Secrets Scan
4. Build
5. Unit Testing
6. SCA (Software Composition Analysis)
7. SAST (Static Application Security Testing)
8. Dockerization
9. Image Scan
10. Sign Artifact
11. Push to Artifact Repository
12. Trigger Continuous Deployment (CD)

## Continuous Delivery (CD)
**Pipeline:**
1. Deploy to staging / test environment
2. DAST (Dynamic Application Security Testing)
3. Integration Tests
4. IaC Scan (Infrastructure as Code)
5. Secrets Check
6. Approve for Production
7. Production Deployment
8. Runtime Security
9. Monitoring & Feedback

## Testing Types
- **SIT** – System Integration Testing
- **Types of Unit Testing:** e.g., functional, regression, mock testing, boundary testing  
- **Types of Artifacts:** e.g., JARs, WARs, Docker images, binaries

## Code Coverage
- **Definition:** Code coverage measures how much of your source code is executed when automated tests (unit, integration, etc.) are run.  
- **Types of Code Coverage:**  
  - Line Coverage  
  - Branch Coverage  
  - Function Coverage  
  - Statement Coverage

## Continuous Delivery vs Continuous Deployment
- **Continuous Delivery:**  
  SIT → Performance Testing → DAST → Approve → Prod Deploy (optional)  
  Additional: NLP testing, Alpha/Beta testing

- **Continuous Deployment:**  
  SIT → Performance Testing → DAST → Prod Deploy (automatic, no manual approval)


## Linux

**Kernel:** Acts as an adapter between hardware (keyboard, CPU, monitor, printer, hard disk, etc.) and software.  
- **Kernel Manages:**  
  - CPU  
  - Memory  
  - I/O devices  


## AWS Console Basics

### How to Create an EC2 Instance
- **Size:** Determines CPU, RAM, and instance type  
- **Key Pair:** For SSH access  
- **VPC (Virtual Private Cloud):** Defines network boundary  
- **Subnet:** Smaller network inside VPC  
- **IP Addresses:**  
  - **Private IP:** Internal AWS communication, not internet-accessible  
  - **Public IP:** Internet-accessible, assigned automatically (changes on stop/start)  
  - **Elastic IP:** Static public IP, can attach/detach to any instance  

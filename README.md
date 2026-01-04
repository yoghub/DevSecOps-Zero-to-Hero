# DevSecOps-Zero-to-Hero

Day 1: The Mindset Shift & Threat Modeling

Focus: Understanding the "Sec" in DevSecOps and planning before coding.

Concepts:

What is DevSecOps? (Shift Left vs. Shield Right).

The 2026 Landscape: AI-driven attacks vs. AI-driven defense.¯¯¯

Threat Modeling: Using the STRIDE framework.

Tool Spotlight: OWASP Threat Dragon or PyTM.

Hands-on Lab: Perform a threat model for a simple 3-tier web application.

Day 2: Application Security (SAST & SCA)

Focus: Securing the code and the supply chain (dependencies).

Concepts:

SAST (Static Application Security Testing): Scanning your own code.

SCA (Software Composition Analysis): Finding vulnerabilities in Open Source libraries.

The "Billion Dollar" Problem: Handling Transitive Dependencies.

Tool Spotlight: Snyk (for SCA) and SonarQube (for SAST).

Hands-on Lab: Integrate Snyk and SonarQube into a GitHub Action/GitLab pipeline to fail builds on "High" vulnerabilities.

Day 3: Secret Management & Infrastructure as Code (IaC) Security

Focus: Preventing credential leaks and securing your Terraform/Bicep code.

Concepts:

Secret Sprawl: Why .env and hardcoded keys are a disaster.

IaC Scanning: Catching misconfigured S3 buckets or open Security Groups before deployment.

Tool Spotlight: TruffleHog (Secret scanning) and Checkov or KICS (IaC scanning).

Hands-on Lab: Scan a "leaky" Terraform repo and implement HashiCorp Vault for dynamic secret injection.

Day 4: Container & Kubernetes Security

Focus: Securing the ship (Docker) and the harbor (K8s).

Concepts:

Distroless images and multi-stage builds.

Image Linting: Finding "root" users and insecure instructions.

Kubernetes Admission Controllers and Network Policies.

Tool Spotlight: Trivy (Image scanning) and Hadolint (Docker linting).

Hands-on Lab: Scan a Docker image for CVEs and deploy a "Secure-by-Default" Pod to a K8s cluster.

Day 5: Dynamic Testing (DAST) & API Security

Focus: Testing the running application for real-world exploits.

Concepts:

DAST (Dynamic Application Security Testing): Attacking the app like a hacker.

OWASP Top 10 (2026 Updates): Injection, Broken Access Control, etc.

Securing REST & GraphQL APIs.

Tool Spotlight: OWASP ZAP (Automation) or StackHawk.

Hands-on Lab: Run an automated ZAP baseline scan against a running staging environment and generate a PDF report.

Day 6: Runtime Security & Compliance as Code

Focus: Monitoring what happens AFTER deployment and staying compliant.

Concepts:

Runtime Security: Detecting drift and suspicious behavior (e.g., a shell opening in a container).

eBPF: The secret sauce of modern cloud-native security.

Compliance (SOC2/GDPR) as an automated check.

Tool Spotlight: Falco (Runtime detection) and Prowler (AWS/Azure/GCP auditing).

Hands-on Lab: Set up Falco to alert on Slack whenever someone runs apt-get install inside a production container.

Day 7: The Grand Finale – Building the Ultimate Pipeline

Focus: Bringing it all together and the DevSecOps Career Roadmap.

The Master Project: Build a "Golden Pipeline" that includes:

Secret Scan (Pre-commit).

SAST/SCA (Build phase).

IaC Scan (Provision phase).

DAST (Post-deploy phase).

AI Fixes: Use AI (like GitHub Copilot or Snyk AI) to auto-remediate a found bug.

Career Guidance: Certifications (CASE, CND, DevSecOps Foundation), resume tips, and the future of the role.

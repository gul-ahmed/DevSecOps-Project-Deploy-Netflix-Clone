# DevSecOps-Project-Deploy-Netflix-Clone

The seamless deployment of a Netflix clone application, hosted on Amazon Web Services (AWS) EC2 instances within Docker containers. The Continuous Integration and Continuous Deployment (CI/CD) pipeline using Jenkins, ensuring efficient and automated code delivery.

To monitor the application's performance and security, Prometheus and Grafana have been integrated. Prometheus collects metrics from various endpoints, while Grafana provides a visually appealing dashboard for real-time monitoring. Node Exporter enhances visibility by collecting system metrics.

In addition, security measures have been fortified with OWASP, ensuring that the application adheres to best practices and safeguards against potential vulnerabilities.

# Phase 1:
Utilizing a t2.large AWS EC2 instance to host Jenkins, SonarQube, and Trivy.

### **Jenkins:**

Jenkins is an open-source automation server that facilitates the continuous integration and continuous delivery (CI/CD) of software development projects. It automates the building, testing, and deployment processes, allowing developers to focus on writing code rather than managing repetitive tasks. Jenkins supports a wide range of plugins, enabling integration with various tools and technologies. It plays a crucial role in streamlining the software development lifecycle, providing a scalable and customizable platform for automating and orchestrating development workflows.

### **SonarQube:**

SonarQube is an open-source platform designed for continuous inspection of code quality. It provides static code analysis to detect bugs, security vulnerabilities, and code smells in various programming languages. SonarQube offers detailed reports and visualizations, empowering development teams to maintain high code quality standards throughout the software development lifecycle.

### **Trivy:**

Trivy is a comprehensive and lightweight open-source vulnerability scanner for container images. It specializes in detecting security vulnerabilities in the dependencies and packages within containerized applications. Trivy supports various container image formats and package managers, making it an essential tool for ensuring the security of containerized environments. Its fast and straightforward approach enables integration into CI/CD pipelines, helping to identify and address vulnerabilities early in the development process.

**Step 1:**
- Launch an Ubuntu-based (Ubuntu 22.04) EC2 instance on AWS.
- Connect to the instance using SSH.

**Step 2:**
- Update all the packages and then clone the code.
- Clone your application's code repository onto the EC2 instance:
```
git clone https://github.com/N4si/DevSecOps-Project.git
```

# CyberReconX

## Ultimate OSINT Reconnaissance & Attack Surface Mapping Toolkit

<div align="center">
    <img src="https://i.ibb.co/PGKRLfw8/Screenshot-2025-02-27-190329.png" alt="CyberReconX Dashboard Screenshot" width="800" />
</div>

[![Visual Studio](https://badgen.net/badge/icon/visualstudio?icon=visualstudio&label)](https://visualstudio.microsoft.com)
[![Website shields.io](https://img.shields.io/website-up-down-green-red/http/shields.io.svg)](https://infosecsamurai.github.io/CyberReconX/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Open Issues](https://img.shields.io/github/issues/InfosecSamurai/CyberReconX.svg)](https://github.com/InfosecSamurai/CyberReconX/issues)
[![Open Pull Requests](https://img.shields.io/github/issues-pr/InfosecSamurai/CyberReconX.svg)](https://github.com/InfosecSamurai/CyberReconX/pulls)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![GitHub stars](https://badgen.net/github/stars/Naereen/Strapdown.js)](https://GitHub.com/Naereen/StrapDown.js/stargazers/)
[![Buymeacoffee](https://badgen.net/badge/icon/buymeacoffee?icon=buymeacoffee&label)](https://buymeacoffee.com/infosecsamurai)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [API Configuration](#api-configuration)
- [Using the Scanner](#using-the-scanner)
- [Example Vulnerabilities](#example-vulnerabilities)
- [Technologies Detected](#technologies-detected)
- [Screenshots](#screenshots)
- [Installation](#installation)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)
- [Contact Information](#contact-information)

## Overview
CyberReconX is an all-in-one OSINT reconnaissance toolkit that enables users to perform comprehensive scans and analysis on target domains and IP addresses. This web-based application is hosted entirely on GitHub Pages and requires no backend setup, making it incredibly easy to use for security professionals and enthusiasts alike.

## Features
- **User-Friendly Dashboard**: A clean and intuitive main dashboard where users can input either a URL or an IP address of the target.
- **Reconnaissance Sections**:
  - **OSINT Collection**: Aggregate data from various open-source intelligence sources.
  - **Subdomain Enumerator**: Discover all subdomains associated with the target domain.
  - **Dark Web Lookup**: Search for potential data breaches or leaks on the dark web.
  - **Username Enumerator**: Identify usernames associated with the target from multiple platforms.
  - **Port Scanning**: Identify open ports on the target, providing valuable information about services running.
  - **Phishing Analysis**: Assess phishing risk for associated domains and services.

- **Reconnaissance Output**: Once the scan is complete, results are displayed in a structured format, highlighting:
  - **Domains and Subdomains**: Status of each target with active/inactive states and corresponding IPs.
  - **Open Ports**: Ports that are accessible for each domain/subdomain.
  - **Vulnerabilities**: A comprehensive list displaying vulnerabilities found, their severity, affected assets, and suggested remediations.

- **Attack Surface Map**: Visual representation of the scanned network, showcasing the relationships between the target and its assets.
- **Security Report Generation**: Generate a downloadable security report that summarizes the findings, including:
  - **Executive Summary**: Overall insights into the reconnaissance session.
  - **Domain/Subdomain Analysis**: List of domains and subdomains scanned.
  - **Vulnerability Assessment**: Details about discovered vulnerabilities, including severity, descriptions, and remediation steps.

- **Export Functionality**: An export button allows users to download scan results in a structured `.json` format for further analysis in any JSON viewer.

## API Configuration
To enable full functionality, the toolkit utilizes several APIs:
- **Shodan**: For port scanning and service detection.
- **SecurityTrails**: For subdomain enumeration.
- **Hunter.io**: For scraping email addresses associated with the target.
- **VirusTotal**: For detecting technologies and vulnerabilities related to domains.

### API Key Configuration
1. Click on the **API Settings** button located in the top right corner of the dashboard.
2. Enter your API keys for Shodan, SecurityTrails, Hunter.io, and VirusTotal into the respective fields.
3. Save your API keys to enable full scanning functionality.

**Note**: Your API keys are securely stored in your browser's local storage and are not shared with our servers.

## Using the Scanner
1. **Input Target**: Enter the target domain (e.g., `example.com`) or IP address (e.g., `192.168.1.1`) in the designated input box on the dashboard.
2. **Select Scan Options**: Choose the scan depth and mode (Passive, Active, or Aggressive).
3. **Start the Scan**: Click the "Start Reconnaissance" button to initiate the scanning process.
4. **Monitor the Output**: Monitor the terminal for ongoing scan updates and results.
5. **View Results**: Once the scan is complete, view results in structured output. An attack surface map will also be generated for visual analysis.
6. **Generate Report**: Click the “Generate Report” button to create a detailed security report.
7. **Export Results**: Use the “Export Results” button to create a downloadable `.json` file of your scan results.

## Example Vulnerabilities
The toolkit identifies various vulnerabilities, providing specific details such as:
1. **HTTP Without HTTPS**
   - **Severity**: Low
   - **Description**: Site is accessible over unencrypted HTTP without HTTPS available.
   - **Remediation**: Implement HTTPS with valid SSL/TLS certificates.

2. **Exposed Admin Interface**
   - **Severity**: Medium
   - **Description**: Administrative interface exposed to the public.
   - **Remediation**: Restrict access to admin interfaces with IP filtering or VPN.

## Technologies Detected
The toolkit will also report on technologies in use for a given domain, including:
- **Technology**: HTTP
- **Version**: 1.1
- **Category**: Web Server
- **Vulnerabilities**: Lists any vulnerabilities detected related to the technology.

## Screenshots
The following images showcase the interface and outputs of the CyberReconX toolkit:

<div align="center">
    <img src="https://i.ibb.co/h1ckCcvQ/Screenshot-2025-03-01-153148.png" alt="Main Dashboard" width="800" /><br>
    <img src="https://i.ibb.co/kgrjBqCj/Screenshot-2025-03-01-153132.png" alt="API Configuration" width="800" /><br>
    <img src="https://i.ibb.co/DDxW5jFX/Screenshot-2025-03-01-153213.png" alt="Reconnaissance Modules" width="800" /><br>
    <img src="https://i.ibb.co/mr6Czgxf/Screenshot-2025-03-01-153110.png" alt="Reconnaissance Output" width="800" /><br>
    <img src="https://i.ibb.co/5hj8TSv6/Screenshot-2025-03-01-153359.png" alt="Reconnaissance Results (Domain & Subdomains)" width="800" /><br>
    <img src="https://i.ibb.co/Xf92jwYN/Screenshot-2025-03-01-153409.png" alt="Reconnaissance Results (Potential Vulnerabilities)" width="800" /><br>
    <img src="https://i.ibb.co/zhRsFNKN/Screenshot-2025-03-01-153443.png" alt="Reconnaissance Results (Technologies)" width="800" /><br>
    <img src="https://i.ibb.co/5WH374mh/Screenshot-2025-03-01-150418.png" alt="Security Report" width="800" />
</div>

## Installation
Clone the repository and host it using GitHub Pages or a local server:
```bash
git clone https://github.com/InfosecSamurai/CyberReconX.git

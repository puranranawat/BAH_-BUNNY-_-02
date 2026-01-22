# Task 4.3 – Security

## 1. Overview
The goal of this section is to identify important cyber security risks for Truelec and reduce them. First, we completed a risk assessment using the unit template. Then, we selected the highest risk data asset and recommended three security controls to protect it.

## 2. Assets Identified

### 2.1 Hardware Assets
Truelec uses many hardware assets such as:
- Routers and switches
- Firewall devices
- Servers for booking application
- WiFi access points
- CCTV cameras
- RFID scanners and IoT devices
- Staff computers and laptops

### 2.2 Software Assets
Truelec uses software assets such as:
- Server operating systems
- Booking application
- Firewall software/firmware
- Remote access VPN software
- Monitoring and logging tools

### 2.3 Data Assets (Minimum 4)
Truelec handles important data including:
- Customer personal information (name, email, phone)
- Booking records and reservation details
- Payment-related data (transaction details)
- Staff login credentials and access roles
- CCTV video footage

### 2.4 People and Process Assets
Truelec also depends on:
- Staff members
- Managers
- IT administrator
- Helpdesk process for password reset and access approval

## 3. Risk Assessment Method
We completed the cyber security risk assessment using the unit-provided template. Risks were rated based on likelihood and impact. We identified threats and vulnerabilities affecting each asset. We covered at least 8 threat categories as required and included multiple data assets.

## 4. Risk Assessment Results Summary
The risk assessment identified several high risks for Truelec. The main risks included phishing attacks, weak passwords, misconfigured WiFi, malware infections, and unauthorized access to customer data.

| Risk ID | Asset | Threat | Vulnerability | Likelihood | Impact | Risk Rating |
|--------|-------|--------|--------------|------------|--------|------------|
| R1 | Customer Data | Data breach | Weak access control | High | High | Extreme |
| R2 | Booking Server | Malware | No patching plan | Medium | High | High |
| R3 | WiFi Network | Unauthorized access | Weak guest WiFi isolation | Medium | Medium | Medium |
| R4 | Staff Accounts | Phishing | Low security awareness | High | Medium | High |

## 5. TVA Matrix Evidence
TVA matrix screenshots are included below as evidence from the risk assessment spreadsheet.
(Insert screenshots here)

## 6. Highest Risk Data Asset Selected
The highest risk data asset selected is: <<HIGHEST_RISK_DATA_ASSET>>.  
This data is critical because it contains sensitive customer information. If this data is stolen or leaked, it can cause identity theft, financial loss, and serious damage to Truelec’s reputation. It can also lead to legal and compliance problems.

## 7. Security Controls Recommendation (3 Controls)

### Control 1: Multi-Factor Authentication (MFA)
- Control source: Unit lecture / NIST SP800-53
- How it reduces risk: MFA adds an extra login step so attackers cannot easily access accounts even if passwords are stolen.
- Implementation in Truelec network: Enable MFA for all admin accounts, server logins, and cloud dashboards.
- Where applied: HQ and branch admin accounts, booking servers, cloud portal.
- Disadvantages: Some users may find it slightly slower to login.

### Control 2: Network Segmentation using VLANs + Firewall Rules
- Control source: Unit lecture / NIST SP800-53
- How it reduces risk: It prevents attackers from moving freely inside the network after gaining access.
- Implementation in Truelec network: Keep servers, staff, guest WiFi, and IoT devices in separate VLANs and apply firewall ACL rules.
- Where applied: HQ and branch networks, firewall/router.
- Disadvantages: Requires correct configuration and maintenance.

### Control 3: Central Logging and Monitoring
- Control source: Unit lecture / NIST SP800-53
- How it reduces risk: Logging helps detect attacks early and supports incident response.
- Implementation in Truelec network: Enable logs on firewall, servers, and VPN. Store logs in a secure location and review regularly.
- Where applied: HQ servers and firewall, branch router/firewall.
- Disadvantages: Requires storage space and monitoring time.

## 8. Conclusion
In conclusion, the risk assessment helped identify major cyber security risks for Truelec. The selected security controls reduce the risk of customer data compromise and improve overall network security. These controls are practical and can be implemented without heavy disruption to daily business work.

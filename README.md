## LAN/WLAN/WAN Migration – (Cisco Catalyst to Meraki Cloud SD-WAN)

📘Project Description

The LAN/WLAN/WAN Migration Project modernizes legacy Cisco Catalyst infrastructure by transitioning to a Meraki Cloud SD-WAN architecture, integrating Zscaler Cloud Security, Microsoft Azure AD, and Rapid7 MDR for comprehensive visibility, security, and cloud-based management.
This transformation supports over 600 users across two operational sites, enabling seamless LAN, WLAN, and WAN communication through a unified cloud-managed platform. The design prioritizes high availability, zero-trust security, and scalability for future cloud expansion.

🎯 Objectives
- Migrate from on-prem Cisco Catalyst switches and routers to Meraki Cloud SD-WAN.
- Enhance network visibility and performance through cloud-based monitoring
- Implement Zscaler for advanced internet and SSL traffic inspection
- Integrate Azure AD for identity-driven access control and single sign-on (SSO)
- Enable Rapid7 MDR for threat intelligence and endpoint correlation
- Establish inter-site VPN tunnels with automatic failover for resilience

⚙️ System Architecture Overview
# Core Components
- LAN Layer: Meraki MS Series Switches (replacing Cisco Catalyst)
- WLAN Layer: Meraki MR Access Points (secure roaming, WPA3 Enterprise)
- WAN Layer: Meraki MX SD-WAN Devices (HA mode, Auto-VPN, cloud control)
- Security Layer: Zscaler Internet Access for real-time inspection and DLP
- Identity Management: Azure Active Directory with MFA and SSO
- Threat Detection: Rapid7 MDR for continuous endpoint threat analytics
- Cloud Management: Meraki Dashboard for centralized orchestration and analytics



<img width="1163" height="339" alt="image" src="https://github.com/user-attachments/assets/c2378b15-1b51-40d1-afd4-e3ee2acf269c" />


🚀 Implementation Phases
**Phase 1: Assessment & Design**
- Conducted site bandwidth and network topology assessment
- Defined VLAN segmentation and QoS policies
- Reviewed compliance and Zscaler integration requirements

**Phase 2: Deployment & Configuration**
- Replaced Cisco Catalyst switches with Meraki MS series
- Configured Meraki MR access points with SSIDs and WPA3 authentication
- Deployed MX SD-WAN edge devices in high-availability (HA) mode

**Phase 3: Integration & Testing**
- Integrate traffic with Zscaler for content inspection
- Sync identity roles and policies from Azure AD
- Link Rapid7 MDR for real-time monitoring and alerting

**Phase 4: Optimization & Monitoring**
- Enable NetFlow and application analytics
- Configure alerting for bandwidth utilization and device status
- Conduct performance tuning and firmware upgrades

🔐 Security Architecture
- **Zero-Trust Access**: Enforced via Azure AD Conditional Access and MFA
- **Traffic Inspection**: All outbound traffic filtered through Zscaler Cloud Proxy
- **RBAC**: Fine-grained admin roles assigned via Azure AD groups
- **Threat Detection**: Rapid7 MDR continuously correlates network and endpoint logs

📈 Business Impact
| Outcome | Impact |
|---------|-----------|
| **Reduced Downtime**	| Cloud-managed auto-failover ensures 99.9% uptime |
| **Improved Security** | Zscaler + Rapid7 MDR enhance visibility and protection |
| **Simplified Management** |	Centralized Meraki Dashboard eliminates manual CLI |
| **Cost Efficiency** |	SD-WAN reduces MPLS dependency and maintenance cost |
| **Future-Ready** | Infrastructure	Scalable for multi-cloud and IoT integration |

🧑‍💻**Access Control**
- Only Azure AD-authenticated users can access the Meraki Dashboard
- MFA is mandatory for all privileged accounts
- Device compliance and access policies enforced via Conditional Access

📊# Monitoring & Reporting
- Meraki Dashboard: Live network topology and client analytics
- Zscaler Portal: Threat posture and policy performance reports
- Rapid7 MDR: Incident response tracking and security analytics
- Weekly Reports: Summaries auto-generated for IT leadership review

⚡ Scalability & Future Enhancements
-  Extend Meraki SD-WAN templates to new branch offices
-  Automate configurations using Terraform and Ansible
-  Integrate Power BI dashboards for performance visualization
-  Evaluate Azure Virtual WAN for expanded global coverage

💼 Business Value Summary

The migration from Cisco Catalyst to Meraki Cloud SD-WAN has established a secure, scalable, and cloud-native enterprise network. By integrating Zscaler, Azure AD, and Rapid7 MDR, the organization achieved:
- 70% faster troubleshooting and configuration rollout
- Enhanced user experience through optimized routing
- Centralized visibility and compliance reporting
- Future-proof foundation for multi-site and hybrid cloud environments

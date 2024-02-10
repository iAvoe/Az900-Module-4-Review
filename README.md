# Az900-Module-4-Review

## Azure Security features

### Microsoft Defender for Cloud
- A monitoring service app that provides protection across Azure & on-premise datacenters
- Provides security recommendations
- Detect & block malware
- Analyze & identify potential attacks
- Just-in-time access control for ports
- Monthly payment plan required

### Defender for Cloud Components
- **Secure Score**:
  - Aggregate all security findings into one score
  - Microsoft cloud security benchmark (MCSB) standard is applied by default
- **Multi-cloud coverage**:
  - Most feature including security score supports Azure, AWS, GCP (Google Cloud)
- **Advanced Cloud Security Posture Management**:
  - Identify weaknesses in security posture
  - *Security Governance* to drive actions to improve security
  - *Regulatory Compliance* to standarize environment and configuration
  - *Cloud security explorer* to build a comprehensive view of environment
- **Data-aware Security Posture**:
  - Auto-discovers datastores that has sensitive data
  - Helps reduce risk of data breaches
- **Attack path analysis**:
  - Model traffic on your network to identify potential risks before user make changes
- **Microsoft Entra Permissions Management**:
  - Provide comprehensive visibility and control over permissions for any identity

### Using Defender for Cloud
- **Policy Compliance**: Run policies across management groups, subscriptions, or tenants
- **Continuous Assessments**: Assess new and deployed resources to ensure that they are configure properly
- **Tailored Recommendations**: Recommendations based on existing workload with instructions on how to implement them
- **Threat Protection**: Analyze attempted threats through alerts & impacted resource reports

*Lab - Monitor and Resolve Security Issues by Using Security Center*

### Resource hygiene

-----

### Key Vault
- Stores application secrets in a centralized cloud location
- Controls access permissions & access logging
  - Secrets management
  - Key management
  - Certificate management
  - Storing secrets backed by hardware security modules (HSMs)

*Lab - Manage Encryption by Using an Azure Key Vault*

### Microsoft Sentinel
- A security information & event management (SIEM) solution
- Provides security analytics, threat intelligence across an enterprise
- *Integrations:*
  - Microsoft 365 Defender
  - Azure Active Directory
  - Azure Advanced Threat Protection
  - Microsoft Cloud App Security

### Azure Dedicated Hosts
- Provide physical servers that host Azure VMs that is for a singal workload
- Provides hardware isolation at server level
- Controls over maintenance event timing
- Aligned with Azure Hybrid Use Benefits

-----

<br>

## Azure network security
- A layered multi-level protection approach similar to OSI levels
- Attacks against one layer are isolated from subsequent layers

### Shared Security
- Migrating from customer to cloud datacenters shifts the responsibility for security
- Security becomes a shared concern as the on-premise data
- **Service model dependent:**

| Responsibility                        | On-Premises | IaaS model  | PaaS model  | SaaS model  |
|---------------------------------------|-------------|-------------|-------------|-------------|
| `Data, governance & Rights Mgmt.    ` | Customer    | Customer    | Customer    | Customer    |
| `Client endpoints                   ` | Customer    | Customer    | Customer    | Customer    |
| `Account & access management        ` | Customer    | Customer    | Customer    | Customer    |
| `Identity & directory infrastructure` | Customer    | Customer    | *Ms*/Cs     | *Ms*/Cs     |
| `Application                        ` | Customer    | Customer    | *Ms*/Cs     | *Microsoft* |
| `Network Controls                   ` | Customer    | Customer    | *Ms*/Cs     | *Microsoft* |
| `Operating System                   ` | Customer    | Customer    | *Microsoft* | *Microsoft* |
| `Physical Hosts                     ` | Customer    | *Microsoft* | *Microsoft* | *Microsoft* |
| `Physical Network                   ` | Customer    | *Microsoft* | *Microsoft* | *Microsoft* |
| `Physical Datacenter                ` | Customer    | *Microsoft* | *Microsoft* | *Microsoft* |

-----

### Network Security Groups (NSGs):
- Azure applies default/baseline security rules to new NSGs, Override default rules with new, higher priority rules.
- filter network traffic to and from Azure resources on Azure Virtual Networks
- Set in-outbound rules by destination IP, ports, and protocols
- Add multiple rules, as needed, within subscription limits

*Lab - Implement a Network Security Group*

### Azure Firewall
- A stateful, managed Firewall as a Service (FaaS)
- Grants/denies server access based on originating IP
- Applies in-outbound traffic filtering rules
- Built-in high availability
- Unrestricted cloud scalability
- Uses Azure Monitor logging

### Azure Application Gateway
- Provides a Web Application Firewall (WAF)
- WAF provides centralized, inbound protection for web apps

### DDoS protection
- Sanitizes unwanted network traffic before it impacts service availability
- Basic service tier is automatically enabled in Azure
- Standard service tier adds mitigation capabilities
  - tuned to protect Azure Virtual Network resources

-----

### Defense in depth
- NSGs + Azure Firewall
- **Perimeter layer:**
  - By Azure DDoS Protection + Azure Firewall
  - Protects network boundaries
- **Networking layer:**
  - By Network Security Group (NSG)'s in-outbound rules
  - Permits traffic to pass between networked resources

-----

<br>

## Quiz


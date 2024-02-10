# Az900-Module-4-Review

## Azure Security features

### Microsoft Defender for Cloud
- A monitoring service app that provides protection across Azure & on-premise DCs
   - DC: datacenter
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

### Resource hygiene

-----

### Key Vault
- Stores application secrets in a centralized cloud location
- Controls access permissions & access logging
  - Secrets management
  - Key management
  - Certificate management
  - Storing secrets backed by hardware security modules (HSMs)
- *Lab - Configure key valut:*
  - Resource group --> Create --> New Key Valut --> Bind to Resource Group & Name key valye --> Create --> Created Key Vault --> Keys --> Create Keys
  - Resource group --> Storage Account --> Security + networking --> Encryption --> Encryption type --> Customer Managed Keys --> Select keys --> Bind created key vault & created key

### Microsoft Sentinel
- A security information & event management (SIEM) solution
- Provides security analytics, threat intelligence across an enterprise
- *Integrations:*
  - Microsoft 365 Defender
  - Azure Active Directory
  - Azure Advanced Threat Protection
  - Microsoft Cloud App Security

Dedicated Hosts

-----

<br>

## Azure network security

Defense in depth

-----

Network Security Groups

Firewalls

-----

DDoS protection

-----

<br>

## Quiz


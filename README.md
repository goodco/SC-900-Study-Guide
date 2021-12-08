

## Describe the Concepts of Security, Compliance, and Identity (10-15%)

### Describe security and compliance concepts & methodologies

| Methodologies| Description |
|---|---|
| [Zero-Trust methodology](https://docs.microsoft.com/en-us/security/zero-trust/) | Zero Trust model assumes breach and verifies each request as though it originated from an uncontrolled network. Regardless of where the request originates or what resource it accesses, the Zero Trust model teaches us to "never trust, always verify." The Zero Trust model has three principles which guide and underpin how security is implemented. These are: verify explicitly, least privilege access, and assume breach. <br/> **1 - Verify explicitly**. Always authenticate and authorize based on the available data points, including user identity, location, device, service or workload, data classification, and anomalies. <br/> **2 - Least privileged access**. Limit user access with just-in-time and just-enough access (JIT/JEA), risk-based adaptive policies, and data protection to protect both data and productivity. <br/> **3 - Assume breach**. Segment access by network, user, devices, and application. Use encryption to protect data, and use analytics to get visibility, detect threats, and improve your security.<br/> <br/> **Six foundational pillars of Zero Trust** <br/> <br/>  In the Zero Trust model, all elements work together to provide end-to-end security. These six elements are the foundational pillars of the Zero Trust model: <br/>    **1 - Identities**  may be users, services, or devices. When an identity attempts to access a resource, it must be verified with strong authentication, and follow least privilege access principles. <br/>  **2 - Devices**  create a large attack surface as data flows from devices to on-premises workloads and the cloud. Monitoring devices for health and compliance is an important aspect of security. <br/>   **3 - Applications**  are the way that data is consumed. This includes discovering all applications being used, sometimes called Shadow IT because not all applications are managed centrally. This pillar also includes managing permissions and access. <br/>   **4 - Data**  should be classified, labeled, and encrypted based on its attributes. Security efforts are ultimately about protecting data, and ensuring it remains safe when it leaves devices, applications, infrastructure, and networks that the organization controls. <br/>  **5 - Infrastructure**, whether on-premises or cloud based, represents a threat vector. To improve security, you assess for version, configuration, and JIT access, and use telemetry to detect attacks and anomalies. This allows you to automatically block or flag risky behavior and take protective actions. <br/>   **6 - Networks**  should be segmented, including deeper in-network micro segmentation. Also, real-time threat protection, end-to-end encryption, monitoring, and analytics should be employed.<br/>![The Zero Trust model](https://docs.microsoft.com/en-us/learn/wwl-sci/describe-security-concepts-methodologies/media/2-zero-trust-pillars-v2.png)|
| [Shared responsibility model](https://docs.microsoft.com/en-us/learn/modules/describe-security-concepts-methodologies/3-describe-shared-responsibility-model)  | [Reference AZ-900](https://github.com/RickKotlarz/az-900/blob/master/az900.md#shared-responsibility-model-in-the-cloud) |
| [Defense in Depth](https://docs.microsoft.com/en-us/learn/modules/describe-security-concepts-methodologies/4-describe-defense-depth) |Defense in depth is a strategy that employs a series of mechanisms to slow the advance of an attack that's aimed at acquiring unauthorized access to information. Each layer provides protection so that if one layer is breached, a subsequent layer is already in place to prevent further exposure. |
| [Common threats](https://docs.microsoft.com/en-us/learn/modules/describe-security-concepts-methodologies/5-describe-common-threats) |Common threats include:<br/> &bull; **Data breach** -  A data breach is when data is stolen, and this includes personal data.<br/> &bull; **Dictionary attack** - A dictionary attack is a type of identity attack where a hacker attempts to steal an identity by trying a large number of known passwords. Each password is automatically tested against a known username. Dictionary attacks are also known as brute force attacks. <br/> &bull; **Ransomware** - Malware is the term used to describe malicious applications and code that can cause damage and disrupt normal use of devices. Malware can give attackers unauthorized access, which allows them to use system resources, lock you out of your computer, and ask for ransom. <br/> &bull; **Disruptive attacks** - A Distributed Denial of Service (DDoS) attack attempts to exhaust an application's resources, making the application unavailable to legitimate users. DDoS attacks can be targeted at any endpoint that is publicly reachable through the internet. Other common threats include coin miners, rootkits, trojans, worms, and exploits and exploit kits. |
| [Encryption](https://docs.microsoft.com/en-us/learn/modules/describe-security-concepts-methodologies/6-describe-ways-encryption-hashing-secure-data)  | There are two top-level types of encryption: symmetric and asymmetric. **Symmetric encryption** uses the ***same key*** to encrypt and decrypt the data.<br/> **Asymmetric encryption** uses a ***public key and private key pair***. Either key can encrypt data, but a single key can’t be used to decrypt encrypted data. To decrypt, you need a paired key. Asymmetric encryption is used for things like Transport Layer Security (TLS), such as the HTTPS protocol, and data signing. Encryption may protect data at rest, or in transit. <br/>![The concept of symmetric and asymmetric encryption](https://docs.microsoft.com/en-us/learn/wwl-sci/describe-security-concepts-methodologies/media/6-encryption.png)<br/> <br/> **Encryption at rest** also known as, data at rest, is the data that's stored on a physical device, such as a server. It may be stored in a database or a storage account but, regardless of where it's stored, encryption of data at rest ensures the data is unreadable without the keys and secrets needed to decrypt it. If an attacker obtained a hard drive with encrypted data and didn't have access to the encryption keys, they would be unable to read the data. <br/><br/> **Encryption in transit** - Data in transit is the data moving from one location to another, such as across the internet or through a private network. Secure transfer can be handled by several different layers. It could be done by encrypting the data at the application layer before sending it over a network. HTTPS is an example of encryption in transit. Encrypting data in transit protects it from outside observers and provides a mechanism to transmit data while limiting the risk of exposure. <br/> <br/> **Hashing** - uses an algorithm to convert the original text to a unique fixed-length hash value. Each time the same text is hashed using the same algorithm, the same hash value is produced. That hash can then be used as a unique identifier of its associated data. Hashing is different to encryption in that it doesn't use keys, and the hashed value isn't subsequently decrypted back to the original. Hashing is used to store passwords. When a user enters their password, the same algorithm that created the stored hash creates a hash of the entered password. This is compared to the stored hashed version of the password. If they match, the user has entered their password correctly. This is more secure than storing plain text passwords, but hashing algorithms are also known to hackers. ![The concept of hashing](https://docs.microsoft.com/en-us/learn/wwl-sci/describe-security-concepts-methodologies/media/6-hashing-3-inline.png)|
| [Confidentiality, Integrity, Availability (CIA)](https://docs.microsoft.com/en-us/learn/modules/describe-security-concepts-methodologies/4-describe-defense-depth)| **Confidentiality** refers to the need to keep confidential sensitive data such as customer information, passwords, or financial data. <br/> **Integrity** refers to keeping data or messages correct.<br/> **Availability** refers to making data available to those who need it. |
| [Cloud Adoption Framework for Azure](https://docs.microsoft.com/en-us/learn/modules/describe-resource-governance-capabilities-azure/) | The **Microsoft Cloud Adoption Framework (CAF)** for Azure is guidance that provides a proven and consistent methodology for implementing cloud technologies that are designed to help you create and implement business and technology strategies for the cloud based on best practices, documentation, and tools.  <br/> **CAF lifecycle includes the following:** <br/>  **1.	Strategy** - Define business justification and expected outcomes of adoption. <br/> **2.	Plan** - Align actionable adoption plans to business outcomes.   <br/>  **3.	Ready** - Prepare the cloud environment for the planned changes and move resources in. <br/>  **4.	Adopt:** <br/> &nbsp;&nbsp;&nbsp;&nbsp; &bull;  ***Migrate:*** Migrate and modernize existing workloads. <br/> &nbsp;&nbsp;&nbsp;&nbsp; &bull; ***Innovate***: Develop new cloud-native or hybrid solutions.  <br/> **5.	Govern** - Establish a well-managed cloud environment <br/> **6. Manage** - Operations management for cloud and hybrid solutions. <br/> <br/> [What is the Microsoft Cloud Adoption Framework for Azure?](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/overview)|


### Define identity concepts

| Identity concepts | Description
|--|--|
|[Identity as the primary security perimeter](https://docs.microsoft.com/en-us/learn/modules/describe-identity-principles-concepts/3-define-identity-primary-security-perimeter) | The traditional perimeter-based security model is no longer enough. Identity has become the new security perimeter that enables organizations to secure their assets. An identity is how someone or something can be verified and authenticated to be who they say they are. An identity may be associated with a user, an application, a device, or something else. Addressing each of these four pillars is key to a comprehensive and robust identity and access control solution. <br/> <br/> **Four pillars of identity** <br/> Identity is a concept that spans an entire environment, so organizations need to think about it broadly. There's a collection of processes, technologies, and policies for managing digital identities and controlling how they're used to access resources. <br/> <br/> There are four fundamental pillars of identity that organizations should consider when creating an identity infrastructure. <br/> <br/> **1 - Administration** - Administration is about the creation and management/governance of identities for users, devices, and services. As an administrator, you manage how and under what circumstances the characteristics of identities can change (be created, updated, deleted).<br/> **2 - Authentication** - The authentication pillar tells the story of how much assurance for a particular identity is enough. In other words, how much does an IT system need to know about an identity to have sufficient proof that they really are who they say they are? It involves the act of challenging a party for legitimate credentials. Authentication is sometimes shortened to AuthN. <br/> **3 - Authorization** - The authorization pillar is about processing the incoming identity data to determine the level of access an authenticated person or service has within the application or service that it wants to access. Authorization is sometimes shortened to AuthZ. <br/>**4 - Auditing** - The auditing pillar is about tracking who does what, when, where, and how. Auditing includes having in-depth reporting, alerts, and governance of identities. |
| [Authentication](https://docs.microsoft.com/en-us/azure/active-directory/develop/authentication-vs-authorization) (Who are you?) | The process of establishing the identity of a person or service looking to access a resource. It involves the act of challenging a party for legitimate credentials, and provides the basis for creating a security principal for identity and access control use. It establishes if they are who they say they are. |
| [Authorization](https://docs.microsoft.com/en-us/azure/active-directory/develop/authentication-vs-authorization) (What are you allowed to do?) | The process of establishing what level of access an authenticated person or service has. It specifies what data they're allowed to access and what they can do with it. |
| [Identity providers](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/identity-providers) | An _identity provider_ creates, maintains, and manages identity information while providing authentication services to applications. When sharing your apps and resources with external users, Azure AD is the default identity provider for sharing. This means when you invite external users who already have an Azure AD or Microsoft account, they can automatically sign in without further configuration on your part. [Extra stuff I need to read](https://docs.microsoft.com/en-us/azure-stack/operator/azure-stack-identity-overview?view=azs-2102) <br/> <br/> [more info](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/identity-providers) <br/> <br/> list of [external identity providers](https://docs.microsoft.com/en-us/azure/active-directory-b2c/add-identity-provider) |
| [Active Directory](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2003/cc758436(v=ws.10)) | A directory is a hierarchical structure that stores information about objects on the network. A directory service, such as Active Directory Domain Services (AD DS), provides the methods for storing directory data and making this data available to network users and administrators. For example, AD DS stores information about user accounts, such as names, passwords, phone numbers, and so on, and enables other authorized users on the same network to access this information. <br/> <br/> [Overview of Active Directory Domain Services (AD DS)](https://docs.microsoft.com/en-us/windows-server/security/group-managed-service-accounts/active-directory-domain-services-overview) |
| [Concept of Federated Services](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-fed) | Federation enables the access of services across organizational or domain boundaries by establishing trust relationships between the respective domain’s identity provider. With federation, there's no need for a user to maintain a different username and password when accessing resources in other domains. <br/><br/> Federation is a collection of domains that have established trust. The level of trust may vary, but typically includes authentication and almost always includes authorization.  <br/> <br/> You can federate your on-premises environment with Azure AD and use this federation for authentication and authorization. This sign-in method ensures that all user authentication occurs on-premises. This method allows administrators to implement more rigorous levels of access control. Federation with [AD FS](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/ad-fs-overview) and PingFederate is available. |
| [Identity Attacks](https://docs.microsoft.com/en-us/learn/modules/describe-identity-principles-concepts/2-describe-common-identity-attacks?WT.mc_id=esi_studyguide_content_wwl) | **Password-based attacks** - Many password-based attacks employ brute force techniques to gain unauthorized access. In a brute force attack, an attacker will attempt to gain access simply by trying different usernames and password combinations. <br/> <br/> **Phishing** - A phishing attack is when a hacker sends an email that appears to come from a reputable source. The email contains a credible story, such as a security breach, instructing the user to sign in and change their password. Instead of going to a legitimate website, the user is directed to the scammer’s website where they enter their username and password. The hacker has now captured the user’s identity, and their password. <br/> <br/> **Spear phishing** - A spear phishing scam is a variant on phishing. Hackers build databases of information about users, which can be used to create highly credible emails. The email may appear to come from someone in your organization who is requesting information. Although careful scrutiny might uncover the fraud, users may not read it carefully enough and send the requested information or login to the website before they realize the fraud. This practice is called spear phishing because it's highly targeted.|

## Describe the capabilities of Microsoft Identity and Access Management Solutions (30-35%)

### Describe the basic identity services and identity types of Azure AD

|Capabilities Term | Description|
|--|--|
|[Azure Active Directory](https://docs.microsoft.com/en-us/learn/modules/explore-basic-services-identity-types/2-describe-what-azure-active-directory)| Reference AZ-900|
|[Azure AD identities](https://docs.microsoft.com/en-us/learn/modules/explore-basic-services-identity-types/4-describe-identity-types) | **User** - A user identity is a representation of something that's managed by Azure AD. Employees and guests are represented as users in Azure AD. If you have several users with the same access needs, you can create a group. You use groups to give access permissions to all members of the group, instead of having to assign access rights individually. <br/> <br/> **Service principal** - A service principal is a security identity used by applications or services to access specific Azure resources. You can think of it as an identity for an application. <br/> <br/> **Managed identity** A managed identity is automatically managed in Azure AD. Managed identities are typically used to manage the credentials for authenticating a cloud application with an Azure service. <br/>  <br/> There are several benefits to using managed identities, including: <br/> &bull; Application developers can authenticate to services that support managed identities for Azure resources. For a complete list of services, refer to Azure Services that support managed identities. <br/> &bull; Any Azure service that supports Azure AD authentication can use managed identities to authenticate to another Azure service; for example, accessing Azure Key Vault. Managed identities can be used without any extra cost. <br/> <br/>  **Device** - A device is a piece of hardware, such as mobile devices, laptops, servers, or printer. Device identities can be set up in different ways in Azure AD, to determine properties such as who owns the device.|
| [Hybrid identity](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-hybrid-identity) | Today, businesses, and corporations are becoming more and more a mixture of on-premises and cloud applications. Users require access to those applications both on-premises and in the cloud. Managing users both on-premises and in the cloud poses challenging scenarios. Microsoft’s identity solutions span on-premises and cloud-based capabilities. These solutions create a common user identity for authentication and authorization to all resources, regardless of location. We call this hybrid identity.|
| [Different external identity types](https://docs.microsoft.com/en-us/azure/active-directory/external-identities/) (Guest Users) | With External Identities in Azure AD, you can allow people outside your organization to access your apps and resources, while letting them sign in using whatever identity they prefer. Within this framework, Azure AD supports a variety of scenarios from business-to-business (B2B) collaboration to access management for consumer/customer- or citizen-facing applications (business-to-customer, or B2C). ***Azure AD External Identities focuses less on a user's relationship to your organization and more on how the user wants to sign in to your apps and resources.*** <br/> [John Saville YouTube](https://www.youtube.com/watch?v=9P10hgPDRZg)|
[What is a device identity?](https://docs.microsoft.com/en-us/azure/active-directory/devices/overview) | A device identity is an object in Azure Active Directory (Azure AD). This device object is similar to users, groups, or applications. A device identity gives administrators information they can use when making access or configuration decisions. <br/> <br/>There are three ways to get a device identity: <br/> &bull; Azure AD registration  <br/> &bull; Azure AD join  <br/> &bull; Hybrid Azure AD join <br/>  <br/>Device identities are a prerequisite for scenarios like device-based Conditional Access policies and Mobile Device Management with Microsoft Endpoint Manager.|

### Describe the authentication capabilities of Azure AD

| Term | Description |
|--|--|
| [Different authentication methods](https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-methods) | blah |
| [What authentication and verification methods are available in Azure Active Directory?](https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-authentication-methods)  | blah |
| [Choose the right authentication method for your Azure Active Directory hybrid identity solution](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/choose-ad-authn) | blah |
| 
| [Self-service password reset (SSPR)](https://docs.microsoft.com/en-us/azure/active-directory/authentication/tutorial-enable-sspr) | blah |
| [Password protection and management capabilities](https://www.microsoft.com/en-us/security/business/identity-access-management/password-protection) | blah |
| [Azure Multi-Factor Authentication](https://docs.microsoft.com/en-us/azure/active-directory/authentication/concept-mfa-howitworks) | Multi-factor authentication (MFA) provides additional security for your identities by requiring two or more elements for full authentication. These elements fall into three categories: <br/>  - Something you know<br/>  - Something you possess<br/>  - Something you are |
| [Windows Hello for Business](https://docs.microsoft.com/en-us/windows/security/identity-protection/hello-for-business/hello-overview) | blah |

### Describe access management capabilities of Azure AD

| Term | Description |
|--|--|
| [Conditional Access](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview) | Allows access to a resources based on meeting one or more predefined criteria|
| [Uses and benefits of conditional access](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/plan-conditional-access) | blah |
| Benefits of Azure AD roles | BLAH  <br/><br/>[Azure AD roles documentation](https://docs.microsoft.com/en-us/azure/active-directory/roles/)  <br/><br/>  [Azure AD built-in roles](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference) |

### Describe the identity protection & governance capabilities of Azure AD

| Term | Description |
|--|--|
| [Identity governance](https://docs.microsoft.com/en-us/azure/active-directory/governance/identity-governance-overview) | blah |
| [Entitlement management](https://docs.microsoft.com/en-us/azure/active-directory/governance/entitlement-management-overview) | blah|
| [Access reviews](https://docs.microsoft.com/en-us/azure/active-directory/governance/access-reviews-overview) | blah <br/><br/> # [Use Azure Active Directory (Azure AD) Identity Governance to review and remove external users who no longer have resource access](https://docs.microsoft.com/en-us/azure/active-directory/governance/access-reviews-external-users) |
| [Capabilities of Privileged Identity Management(PIM)](https://docs.microsoft.com/en-us/azure/active-directory/privileged-identity-management/pim-configure) | blah |
| [Azure AD Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/overview-identity-protection) | blah |

## Describe the capabilities of Microsoft Security Solutions (35-40%)

### Describe basic security capabilities in Azure

| Term | Description |
|--|--|
| [Network Security Groups (NSG)](https://docs.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview) | NSGs operate at layers 3 & 4, and provide a list of allowed and denied communication to and from network interfaces and subnets. NSGs are fully customizable, and give you the ability to fully lock down network communication to and from your virtual machines. By using NSGs, you can isolate applications between environments, tiers, and services. ***Note: NSGs uses static IP addresses and as your network scales this may become difficult to maintain.*** |
| [Azure DDoS Protection](https://docs.microsoft.com/en-us/azure/ddos-protection/ddos-protection-overview) | DDoS Protection leverages the scale and elasticity of Microsoft’s global network to bring DDoS mitigation capacity to every Azure region. The Azure DDoS Protection service protects your Azure applications by scrubbing traffic at the Azure network edge before it can impact your service's availability. Within a few minutes of attack detection, you are notified using Azure Monitor metrics.<br/><br/> Comes in two versions: <br/> Azure DDoS Protection Basic (*Free*)<br/> Azure DDoS Protection Standard (*provides SLAs for Application and Cost Protection*) <br/><br/> Every property in Azure is protected by Azure's infrastructure DDoS (Basic) Protection at no additional cost and requires no user configuration or application changes. <br/> ![](https://docs.microsoft.com/en-us/azure/ddos-protection/media/ddos-protection-overview/ddos-comparison.png)|
| [Azure Firewall](https://docs.microsoft.com/en-us/azure/firewall/overview) | Azure Firewall is a managed, cloud-based, network security service that protects your Azure Virtual Network resources. It is a fully stateful firewall as a service with built-in high availability and unrestricted cloud scalability. Azure Firewall provides inbound protection for non-HTTP/S protocols. Examples of non-HTTP/S protocols include: Remote Desktop Protocol (RDP), Secure Shell (SSH), and File Transfer Protocol (FTP). It also provides outbound, network-level protection for all ports and protocols, and application-level protection for outbound HTTP/S. |
| [Azure Bastion](https://docs.microsoft.com/en-us/azure/bastion/bastion-overview) | blah |
| [Web Application Firewall](https://docs.microsoft.com/en-us/azure/web-application-firewall/overview) | blah |
| [Azure encrypts data](https://docs.microsoft.com/en-us/azure/security/fundamentals/encryption-overview) | blah |

### Describe security management capabilities of Azure

| Term | Description |
|--|--|
| [Defender for Cloud](https://docs.microsoft.com/en-us/azure/defender-for-cloud/defender-for-cloud-introduction) | Defender for Cloud (formerly called Azure Security Center) is a monitoring service tool that provides threat protection across all of your services both in Azure, and on-premises and in other clouds due to integration with  [Azure Defender](https://aka.ms/azuredefender). Available in two tiers, Free (limited to assessments and recommendations only); Standard (full suite of security-related services including continious monitoring, threat detection and just-in-time access control)<br/>_Usage scenarios:_<br/> &bull; Incident Response (Detect, Assess, Diagnose)<br/>&bull; Implement Recommendations <br/><br/> **Key features include:**<br/>&bull; **Compliance dashboard** - Compares the configuration of your resources against requirements outlined within in industry standards, [regulations](https://docs.microsoft.com/en-us/azure/defender-for-cloud/update-regulatory-compliance-packages), and [benchmarks](https://docs.microsoft.com/en-us/security/benchmark/azure/overview).   <br/>&bull; **Security alerts** - When Defender for Cloud detects a threat in any area of your environment, it generates a security alert. These alerts describe details of the affected resources, suggested remediation steps, and in some cases an option to trigger a logic app in response.  <br/>&bull; **Secure score** - A single score so that you can tell, at a glance, your current security situation (the higher the score, the lower the identified risk level). You can view your overall Secure score across your subscriptions or management groups, depending on the scope you select. The score is calculated based on the ratio between your healthy resources and your total resources and will vary based on subscription selected and the active recommendations on these subscriptions. <br/> &bull; **Resource security hygiene** - Most prevalent recommendations and highest impact recommendations.|
| Azure secure score | see above|
| Benefit and use cases of [Azure Defender](https://azure.microsoft.com/en-us/services/azure-defender/) | Azure Defender, previously the cloud workload protection platform (CWPP), ... blah blah... <br/><br/>[Defender for cloud](https://docs.microsoft.com/en-us/azure/defender-for-cloud/defender-for-cloud-introduction) |
| [Cloud security posture management (CSPM)](https://docs.microsoft.com/en-us/azure/defender-for-cloud/defender-for-cloud-introduction#cloud-security-posture-management-cspm) | blah |
| [Security baselines for Azure](https://docs.microsoft.com/en-us/security/benchmark/azure/baselines/policy-security-baseline) | blah |

### Describe security capabilities of Azure Sentinel

| Term | Description |
|--|--|
| [Concepts of SIEM, SOAR, XDR](https://docs.microsoft.com/en-us/learn/modules/describe-security-capabilities-of-azure-sentinel/)| blah |
| Role and value of [Azure Sentinel](https://docs.microsoft.com/en-us/azure/sentinel/) to provide integrated threat protection | blah <br/><br/> [An integrated approach for  increased SOC efficiency](https://clouddamcdnprodep.azureedge.net/gdc/gdcTIijLy/original) |

### Describe threat protection with Microsoft 365 Defender

| Term | Description |
|--|--|
| [Microsoft 365 Defender services](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/?view=o365-worldwide) | blah |
| [Microsoft Defender for Identity](https://docs.microsoft.com/en-us/defender-for-identity/what-is) (formerly Azure ATP) | blah |
| [Microsoft Defender for Office 365](https://docs.microsoft.com/en-us/microsoft-365/security/office-365-security/overview?view=o365-worldwide) (formerly Office 365 ATP) | blah |
| [Microsoft Defender for Endpoint](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint?view=o365-worldwide) (formerly Microsoft Defender ATP) | blah |
| [Microsoft Cloud App Security](https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/microsoft-cloud-app-security-integration?view=o365-worldwide) | blah |

### Describe security management capabilities of Microsoft 365

| Term | Description |
|--|--|
| [Microsoft 365 Defender portal](https://docs.microsoft.com/en-us/microsoft-365/security/defender/portals?view=o365-worldwide) | blah |
| [How to use Microsoft Secure Score](https://docs.microsoft.com/en-us/microsoft-365/security/defender/microsoft-secure-score?view=o365-worldwide) | blah |
| [Security reports and dashboards](https://docs.microsoft.com/en-us/microsoft-365/security/office-365-security/security-dashboard?view=o365-worldwide) | blah  |
| [Incidents and incident management capabilities](https://docs.microsoft.com/en-us/compliance/assurance/assurance-incident-management) | blah |

### Describe endpoint security with Microsoft Intune

| Term | Description |
|--|--|
| [What Intune is](https://docs.microsoft.com/en-us/mem/intune/fundamentals/what-is-intune) | blah |
| [Endpoint security with Intune](https://docs.microsoft.com/en-us/mem/intune/protect/endpoint-security) | blah |
| [Endpoint security with the Microsoft Endpoint Manager admin center](https://docs.microsoft.com/en-us/mem/endpoint-manager-overview) | blah |

## Describe the Capabilities of Microsoft Compliance Solutions (25-30%)


### Describe the compliance management capabilities in Microsoft

| Term | Description |
|--|--|
| [Offerings of the Service Trust portal](https://docs.microsoft.com/en-us/microsoft-365/compliance/get-started-with-service-trust-portal?view=o365-worldwide) | blah |
| [Microsoft’s privacy principles](https://www.microsoft.com/en-us/trustcenter/privacy/) | Ref to AZ-900|
| [Compliance center](https://docs.microsoft.com/en-us/microsoft-365/compliance/microsoft-365-compliance-center?view=o365-worldwide) | blah |
| [Compliance manager](https://docs.microsoft.com/en-us/microsoft-365/compliance/compliance-manager?view=o365-worldwide) | blah |
| [Use and benefits of compliance score](https://docs.microsoft.com/en-us/microsoft-365/compliance/compliance-score-calculation?view=o365-worldwide) | blah |

### Describe information protection and governance capabilities of Microsoft 365

| Term | Description |
|--|--|
| [Data classification capabilities](https://docs.microsoft.com/en-us/microsoft-365/compliance/data-classification-overview?view=o365-worldwide) | blah |
| [Value of content and activity explorer](https://docs.microsoft.com/en-us/microsoft-365/compliance/data-classification-activity-explorer?view=o365-worldwide) | blah |
| [Sensitivity labels](https://docs.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide) | blah |
| [Retention Polices and Retention Labels](https://docs.microsoft.com/en-us/microsoft-365/compliance/retention?view=o365-worldwide) | blah |
| [Records Management](https://docs.microsoft.com/en-us/microsoft-365/compliance/records-management?view=o365-worldwide) | blah |
| [Data Loss Prevention (DLP)](https://docs.microsoft.com/en-us/microsoft-365/compliance/dlp-overview-plan-for-dlp?view=o365-worldwide) | [Learn about data loss prevention](https://docs.microsoft.com/en-us/microsoft-365/compliance/dlp-learn-about-dlp?view=o365-worldwide) <br/><br/>  [Plan for data loss prevention (DLP)](https://docs.microsoft.com/en-us/microsoft-365/compliance/dlp-overview-plan-for-dlp?view=o365-worldwide%7C)

### Describe insider risk capabilities in Microsoft 365

| Term | Description |
|--|--|
| [Insider risk management solution](https://docs.microsoft.com/en-us/microsoft-365/compliance/insider-risk-management?view=o365-worldwide) | blah |
| [Communication compliance](https://docs.microsoft.com/en-us/microsoft-365/compliance/communication-compliance?view=o365-worldwide) | blah |
| [Information barriers](https://docs.microsoft.com/en-us/microsoft-365/compliance/information-barriers?view=o365-worldwide) | blah |
| [Privileged access management](https://docs.microsoft.com/en-us/microsoft-365/compliance/privileged-access-management-overview?view=o365-worldwide) | blah |
| [Customer lockbox](https://docs.microsoft.com/en-us/microsoft-365/compliance/customer-lockbox-requests?view=o365-worldwide) | Office 365 Customer Lockbox feature which will help a customer to control how a Microsoft support engineer is going to access customer data during a scenario where customers have raised a support request to investigate some service issues related to customers Office 365 tenant. <br/><br/> Office 365 Customer Lockbox allows the customer to Approve or Reject access request made by the Microsoft Support engineers to access customer data. If customers give access by Approving the request, Microsoft Support Engineers will be able to access the data to help customers resolve issues if they deem necessary. |

### Describe the eDiscovery and audit capabilities of Microsoft 365

| Term | Description |
|--|--|
| [Purpose of eDiscovery](https://docs.microsoft.com/en-us/microsoft-365/compliance/ediscovery?view=o365-worldwide) | blah |
| [Capabilities of the content search tool](https://docs.microsoft.com/en-us/microsoft-365/compliance/search-for-content?view=o365-worldwide) | blah |
| [Core eDiscovery workflow](https://docs.microsoft.com/en-us/microsoft-365/compliance/get-started-core-ediscovery?view=o365-worldwide) | blah |
| [Advanced eDiscovery workflow](https://docs.microsoft.com/en-us/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide) | blah |
| [Core audit capabilities of M365](Core%20audit%20capabilities%20of%20M365) | blah |
| [Purpose and value of Advanced Auditing](https://docs.microsoft.com/en-us/microsoft-365/compliance/advanced-audit?view=o365-worldwide) | blah |

### Describe resource governance capabilities in Azure

| Term | Description |
|--|--|
| [Resource locks](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/lock-resources) | As an administrator, you can lock a subscription, resource group, or resource to prevent other users in your organization from accidentally deleting or modifying critical resources. The lock overrides any permissions the user might have. <br/> <br/> You can set the lock level to **CanNotDelete** or **ReadOnly**. *In the portal, the locks are called **Delete** and **Read-only** respectively.* <br/>  &bull; **CanNotDelete** means authorized users can still read and modify a resource, but they can't delete the resource.  <br/> &bull; **ReadOnly** means authorized users can read a resource, but they can't delete or update the resource. Applying this lock is similar to restricting all authorized users to the permissions granted by the **Reader** role.|
| [Azure Blueprints](https://docs.microsoft.com/en-us/azure/governance/blueprints/overview)| Enables cloud architects and central information technology groups to define a repeatable set of Azure resources that implements and adheres to an organization's standards, patterns, and requirements. Azure Blueprints makes it possible for development teams to rapidly build and stand up new environments with trust they're building within organizational compliance with a set of built-in components, such as networking, to speed up development and delivery.<br/> <br/>  Blueprints are a declarative way to orchestrate the deployment of various resource templates and other artifacts such as:<br/> &bull;  Role Assignments <br/> &bull; Policy Assignments <br/> &bull;  Azure Resource Manager templates (ARM templates) <br/> &bull; Resource Groups <br/><br/> [Azure Blueprints documentation](https://docs.microsoft.com/en-us/azure/governance/blueprints/) <br/> [Understand the lifecycle of an Azure Blueprint](https://docs.microsoft.com/en-us/azure/governance/blueprints/concepts/lifecycle)
| [Azure Policy](https://docs.microsoft.com/en-us/azure/governance/policy/overview) and describe its use cases | blah |

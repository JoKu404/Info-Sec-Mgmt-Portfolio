# Chapter 5: Protecting Security of Assets

---

## Domain 2.0: Asset Security

---

### **Identifying and Classifying Information and Assets**

The initial step in ensuring the security of any asset—whether it's information, physical hardware, or software—is **identification and classification**. This process sets the stage for the appropriate management and protection of resources based on their sensitivity, value to the organization, and regulatory requirements.

#### **Data Classification**
Data classification is a process of assigning categories to data based on its level of sensitivity, importance, and the consequences of unauthorized access or loss. Classifying data is not just a regulatory requirement in many cases; it is also a best practice for ensuring that the data receives the protection it deserves.

Common classification categories include:

- **Top Secret:** Information classified as top secret would cause exceptionally grave damage to national or organizational security if disclosed. This level of classification is reserved for the most sensitive data.
  
- **Secret:** Secret data could cause significant damage to national or organizational security if exposed to unauthorized parties. Stringent controls are applied to ensure this data's protection.
  
- **Confidential:** This classification is used for information that could cause some damage but not at a catastrophic level. Still, it requires protection to avoid any negative repercussions.
  
- **Unclassified:** Public information is data intended for wide distribution with no security requirements. It does not require stringent protective measures since its disclosure poses no harm.

The process of data classification often depends on organizational policies and applicable laws and regulations. By establishing clear classification standards, organizations can effectively guide their teams on how data should be handled throughout its lifecycle.

#### **Asset Classification**
Beyond data, organizations also need to classify physical and technological assets such as servers, storage devices, and the hardware used to process sensitive information. The classification of assets should align with the sensitivity of the data they handle. For example, a server processing top-secret data should be classified and handled with security controls suitable for the most critical assets.

Asset classification ensures that physical and digital resources are consistently managed in a way that supports overall data security strategies. It also serves to protect the integrity, confidentiality, and availability of sensitive information processed by these assets.

---

### **Establishing Information and Asset Handling Requirements**

Once an organization has classified its data and assets, it must develop clear guidelines for handling them. Handling requirements ensure that both physical and digital assets are treated according to their classification. Mishandling sensitive data or assets can lead to significant breaches, regulatory penalties, and reputational damage.

#### **Labeling Assets**
Proper labeling is a fundamental part of asset handling. Clearly marked assets help employees understand the sensitivity level and corresponding security controls that must be applied. For example, laptops that are used to process top-secret information should be labeled as such, with physical or digital tags indicating the level of sensitivity. Digital documents should include metadata or watermarks that identify their classification, ensuring that users understand the appropriate handling procedures.

#### **Securing Physical Assets**
When transporting or storing physical media or hardware, encryption and physical security controls must be in place to prevent unauthorized access. For example, backup tapes containing sensitive data should be encrypted and stored in secured, access-controlled environments.

Similarly, when sensitive data is being transmitted across networks, encryption protocols must be used to protect data in transit. Organizations must also establish access control measures to limit who can handle or access these classified assets, preventing accidental exposure or intentional misuse.

#### **Transporting Sensitive Data**
Organizations must implement stringent protocols when transporting classified data, whether across networks or physical locations. Data in transit is particularly vulnerable to interception, which is why encryption is critical. Additionally, policies regarding who can access or transport sensitive data help ensure that the correct personnel are handling the data securely.

---

### **Managing the Data Lifecycle**

Protecting assets and data throughout their lifecycle—from creation to destruction—is vital for maintaining security. The **data lifecycle** encompasses various stages: creation, collection, storage, maintenance, and destruction. Each of these stages presents unique security challenges that require the implementation of specific controls.

#### **Data Roles: Owners, Controllers, Custodians, and Users**
A crucial part of managing the data lifecycle is defining the roles of individuals responsible for handling and protecting data. Clear delineation of roles ensures accountability and effective management.

- **Data Owners:** Data owners hold the ultimate responsibility for the data and its classification. They define who can access the data and determine the security measures required to protect it.
  
- **Data Custodians:** Data custodians are responsible for the day-to-day management of the data, ensuring that it is properly maintained, stored, and backed up according to organizational policies.

- **Data Processors and Controllers:** Particularly in the context of regulations like the **General Data Protection Regulation (GDPR)**, data controllers determine how and why personal data is processed, while data processors handle the data on behalf of controllers.
  
- **Users:** Users are individuals who interact with the data to perform their job functions. They must adhere to the access controls and handling policies set forth by the data owners and custodians.

#### **Data Collection**
The data collection phase is the point at which data is created or received by an organization. It is essential to minimize data collection to only what is necessary for business operations and legal obligations. Collecting excessive or unnecessary data increases the risk of exposure and legal complications.

Data collection policies should also ensure compliance with privacy laws. For example, consent must be obtained when collecting personal data, and organizations must inform users of how their data will be used and protected.

#### **Data Location and Storage**
As organizations increasingly rely on cloud services and off-site storage, understanding the physical and virtual locations of data is critical. Sensitive data stored in the cloud or on external servers must be encrypted both at rest and in transit to prevent unauthorized access. Additionally, organizations must ensure that data is stored in compliance with jurisdictional regulations, especially when it involves cross-border data transfers.

Proper data storage practices include regular backups, the use of secure servers, and the implementation of physical security measures in data centers. Additionally, organizations must ensure that data is not stored longer than necessary, as required by data retention policies.

#### **Data Maintenance**
Data maintenance refers to the continuous care, updating, and management of data throughout its lifecycle. Regular backups, updates to access controls, and the review of data storage practices ensure that sensitive data remains secure. As part of ongoing maintenance, organizations should also perform audits to ensure that data is classified, handled, and protected according to policy.

#### **Data Retention**
Retention policies outline how long data must be kept. These policies are driven by regulatory requirements, business needs, and legal mandates. For instance, **financial records** may need to be stored for seven years, while healthcare data might have different retention periods under **HIPAA**. It is crucial that organizations align their data retention policies with the applicable regulations to avoid compliance issues.

#### **Data Remanence**
**Data remanence** refers to the residual representation of data that remains on storage media after attempts to erase or delete it. Even after data is deleted, traces can remain, potentially allowing attackers to recover sensitive information.

---

### **Data Destruction**

When data is no longer needed, or its retention period has expired, it must be securely destroyed to prevent unauthorized recovery. Simply deleting files or formatting storage devices does not suffice, as data can often be recovered using advanced forensic techniques. Therefore, organizations must employ robust destruction methods.

#### **Data Destruction Techniques**
- **Erasing:** Erasing data removes directory or catalog links to files, but the actual data remains on the disk until overwritten. This method is not secure for sensitive data.
  
- **Clearing (Overwriting):** Overwriting the entire media with random data multiple times (often referred to as a "three-pass overwrite") makes it more difficult for recovery tools to retrieve the original data.
  
- **Purging:** Purging goes beyond clearing by ensuring that data is not recoverable using any known recovery methods. Purging often involves multiple layers of erasure, and it is typically trusted for less sensitive information.
  
- **Degaussing:** This process uses a strong magnetic field to erase data from magnetic media like hard drives or tapes. Degaussing disrupts the magnetic domains of the media, rendering the data unrecoverable. However, this method is ineffective for modern **solid-state drives (SSDs)**, which store data using integrated circuits rather than magnetic fields.
  
- **Physical Destruction:** For the highest level of security, physically destroying the media ensures that data cannot be recovered. Shredding, incineration, and pulverizing are common methods used for this purpose. This method is especially important for media holding **top-secret** data or any information subject to stringent compliance requirements.

#### **Cryptographic Erasure**
When data is encrypted, **cryptographic erasure** (also known as **crypto-shredding**) can be used as a method of data destruction. Instead of physically destroying the media or overwriting the data, the encryption keys are destroyed, rendering the encrypted data unreadable. This method is particularly effective for cloud environments, where physical destruction of the storage media is not an option.

---

### **Ensuring Appropriate Asset Retention**

Asset retention involves more than just storing data—it includes managing hardware and software assets over their useful life. Every asset, whether physical or digital, has a finite lifespan, after which it becomes obsolete or unsupported. Managing these assets through their lifecycle ensures that sensitive information is protected from the moment an asset is introduced to the organization until it is securely decommissioned.

#### **End of Life (EOL) and End of Support (EOS)**
When a hardware or software product reaches its **End of Life (EOL)** or **End of Support (EOS)**, it no longer receives security updates or support from its vendor. Continuing to use EOL/EOS systems introduces significant vulnerabilities, as these systems may no longer be able to defend against emerging threats.

Organizations must have a clear asset management strategy in place to ensure that obsolete systems are replaced before they become a security liability. Furthermore, old hardware that contains sensitive information must be properly decommissioned and destroyed to prevent data leaks.

---
### **Cloud Access Security Broker (CASB)**

As organizations increasingly adopt cloud-based infrastructure and services, securing data in the cloud has become a significant concern. A **Cloud Access Security Broker (CASB)** is a security policy enforcement point placed between cloud service consumers and cloud service providers. The CASB ensures that security policies and controls are consistently applied across cloud services and that the organization’s cloud environment remains secure.

A CASB monitors all cloud activity, enforcing security policies like authentication, encryption, and logging access. It can also detect shadow IT—when employees use unsanctioned cloud services without the IT department’s approval. A CASB addresses four primary pillars:

- **Visibility:** It gives visibility into who is accessing cloud data and how it is being used.
- **Compliance:** Ensures that cloud usage complies with industry regulations (such as GDPR, HIPAA, or PCI DSS).
- **Threat Protection:** Identifies malicious behavior, data breaches, or cyberattacks targeting the cloud.
- **Data Security:** Enforces data encryption and data loss prevention (DLP) policies.

In essence, CASBs act as intermediaries to enforce corporate security policies when users access cloud resources, ensuring that sensitive data remains secure even in cloud environments.

---

### **Tokenization**

**Tokenization** is a method of protecting sensitive data by replacing it with a token—a surrogate value that has no intrinsic meaning or value outside its use. Tokenization is widely used in payment systems and other contexts where personal or financial data must be stored or transmitted securely.

In the case of payment systems, for example, a token replaces the customer’s credit card number. Instead of storing the actual number in a database, the token is stored, and when a transaction is processed, the token is used to retrieve the actual credit card information from a secure, centralized location. This protects the actual data from exposure to attackers who might compromise the database.

Unlike encryption, where the original data can be recovered with a key, tokenization replaces the data entirely with a token that can only be mapped back to the original data in a secure environment. This makes it particularly effective for data protection in scenarios where the actual sensitive data does not need to be processed or stored by third-party systems.

---

### **Anonymization**

**Anonymization** is the process of removing or obfuscating personal data such that the original data subject cannot be identified. It is commonly used in contexts such as medical research, where researchers need access to data sets but do not need to know the identities of the individuals involved. Anonymization ensures that personal identifiers are stripped from the data, protecting the privacy of individuals.

Anonymization differs from pseudonymization in that pseudonymized data can still be linked back to the data subject if necessary. In contrast, properly anonymized data cannot be traced back to the individual. While anonymization is an effective method for protecting privacy, it must be implemented carefully to ensure that there is no possibility of re-identifying individuals through indirect means, such as combining anonymized data sets with other available information.

---

### **Using Security Baselines**

**Security baselines** are predefined sets of security controls that provide a foundational level of protection for an organization’s systems and data. These baselines are tailored to the specific needs and risk profile of an organization, ensuring that minimum security standards are consistently met across the organization’s infrastructure.

A security baseline helps to ensure that all systems are deployed with a minimum level of security, reducing the risk of misconfigurations or security gaps. Baselines are often based on industry standards and frameworks, such as the **NIST SP 800-53** or **ISO 27001**.

Security baselines are typically organized based on the potential impact of a security breach:

#### **Low-Impact System**
Controls for low-impact systems are recommended when the loss of confidentiality, integrity, or availability would have a minimal impact on the organization.
#### **Moderate-Impact System**
Moderate-impact systems require stronger security controls because a loss of confidentiality, integrity, or availability could have a moderate impact on the organization’s operations.
#### **High-Impact System**
High-impact systems require the most stringent security controls because a compromise could result in severe damage to the organization’s mission or result in significant financial, reputational, or operational harm. 

#### **Privacy Control Baseline**
A **privacy control baseline** specifically focuses on protecting Personally Identifiable Information (PII) and sensitive personal data. This baseline is particularly relevant for organizations subject to privacy regulations, such as **GDPR** or **HIPAA**, and includes controls designed to ensure that personal data is collected, processed, and stored securely, with appropriate consent and access control mechanisms in place.

By establishing and enforcing security baselines, organizations can ensure that their systems meet a consistent level of security, reducing the risk of human error or inadequate protection across different departments or systems. Tailoring these baselines to fit the specific risk levels and regulatory requirements of the organization further strengthens the overall security posture.

---

### **Determining Data Security Controls and Compliance**

Ensuring that appropriate security controls are in place is one of the most critical aspects of asset security. These controls protect data from unauthorized access and ensure that the organization complies with legal and regulatory requirements. 

#### **Data States: In Use, In Transit, and At Rest**
Data exists in three states: in use, in transit, and at rest. Each state presents unique security challenges and requires specific controls to protect data.

- **Data in Use:** This refers to data that is actively being processed by applications or residing in memory. **Encryption** can be used to protect data in use, but the challenge lies in ensuring that encryption does not interfere with the functionality of the application.
  
- **Data in Transit:** Data being transmitted across networks—whether internal or external—must be encrypted to prevent unauthorized interception. **Transport Layer Security (TLS)** and **IPsec** are common protocols used to secure data in transit.
  
- **Data at Rest:** Data stored on media, whether on-premises or in the cloud, must be encrypted to protect it from unauthorized access. Strong encryption algorithms, such as **AES-256**, are commonly used to ensure that data remains confidential.

#### **Scoping and Tailoring Security Controls**
Different organizations face different risks depending on their size, industry, and regulatory environment. Therefore, it is crucial to **scope and tailor security controls** based on an organization’s specific needs. The **National Institute of Standards and Technology (NIST) SP 800-53** provides guidance on tailoring controls to meet organizational goals. The process involves adjusting baseline security controls, considering factors such as data sensitivity, threat levels, and applicable laws.

#### **Standards Selection**
Choosing the appropriate security standards is critical to ensuring both compliance and effective protection of sensitive data. Common standards include:

- **Payment Card Industry Data Security Standard (PCI DSS):** This standard applies to organizations handling credit card transactions and outlines specific requirements for securing payment data.
  
- **General Data Protection Regulation (GDPR):** Applicable to any organization processing data belonging to EU citizens, GDPR imposes strict requirements on data privacy and security.
  
- **Health Insurance Portability and Accountability Act (HIPAA):** This U.S. regulation mandates how healthcare providers, insurers, and related organizations must handle **Protected Health Information (PHI)**.

#### **Data Protection Methods**
Multiple technologies and methods exist to protect sensitive data from unauthorized access:

- **Digital Rights Management (DRM):** DRM technologies control access to copyrighted content such as software, music, and movies. DRM systems can prevent unauthorized copying, modification, and redistribution of digital content.
  
- **Data Loss Prevention (DLP):** DLP systems detect and block unauthorized attempts to transfer sensitive data outside of the organization. DLP solutions can monitor email, file transfers, and other forms of communication to ensure compliance with data handling policies.
  
- **Cloud Access Security Broker (CASB):** As more organizations move to cloud-based systems, CASBs are becoming increasingly important. A CASB sits between the organization's infrastructure and the cloud service provider, enforcing security policies, encrypting data, and providing visibility into how cloud-based data is being accessed and used.

---


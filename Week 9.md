# Chapter 13: Managing Identity and Authentication  

---

## Domain 5.0: Identity and Access Management (IAM)  


---

### **Know how physical access controls protect assets.**  

Physical access controls protect assets by limiting and monitoring who can interact with physical systems, facilities, and hardware, thereby preventing unauthorized entry and tampering. These controls are the first line of defense, providing tangible barriers against physical threats such as theft, vandalism, and sabotage.  

Examples of physical access controls include **locks**, **keycards**, **biometric scanners**, **security guards**, and **surveillance systems**. For instance, data centers may use multi-factor authentication for physical entry, requiring both a keycard and fingerprint scan. Critical areas such as server rooms or vaults often feature layered access controls, ensuring that only authorized personnel with a legitimate purpose can enter.  

In addition to preventing unauthorized physical access, these controls are complemented by logging and monitoring mechanisms. Access logs record every entry and exit, enabling organizations to trace incidents and investigate potential breaches. Combining these preventive and detective measures enhances the overall security posture, ensuring that physical assets remain secure and functional.  

---

### **Know how logical access controls protect assets.**  

Logical access controls safeguard digital resources, including data, applications, and systems, by managing user authentication, authorization, and activity monitoring. These controls are designed to ensure that only authorized users can access specific resources under predefined conditions, reducing the risk of data breaches and misuse.  

Key mechanisms include **passwords**, **biometric verification**, **role-based access control (RBAC)**, **multi-factor authentication (MFA)**, and **encryption**. For example, logical access controls might enforce MFA, requiring users to provide both a password and a one-time code from a hardware token. Additionally, tools like **firewalls** and **network access control (NAC)** systems restrict unauthorized devices or IP ranges from accessing a network.  

Activity monitoring complements these measures by tracking user actions and flagging anomalies. For instance, if a user account is accessed from an unfamiliar location, logical controls may trigger an alert or lock the account. This combination of preventive and reactive measures ensures robust protection of digital assets.  

---

### **Know the difference between subjects and objects.**  

In access control terminology, a **subject** is an active entity that interacts with resources, while an **object** is the passive entity being accessed. Subjects initiate actions, such as reading, writing, or modifying data, while objects are the targets of these actions, such as files, databases, or devices.  

For example, in a database system, a subject might be a user who queries a database (object) for specific records. Access control policies determine whether the subject's requested action (e.g., read or write) is permitted based on roles, permissions, or attributes.  

Understanding this distinction is critical for implementing security models like **Discretionary Access Control (DAC)** or **Mandatory Access Control (MAC)**. These models define the rules governing the interactions between subjects and objects, ensuring secure and appropriate access based on organizational policies.  

---

### **Know the components of the AAA model of access control.**  

The **Authentication, Authorization, and Accounting (AAA)** model provides a comprehensive framework for managing access to systems and resources. Each component plays a specific role in ensuring security:  

1. **Authentication**: Verifies a user's identity, ensuring that only legitimate users can access resources. Methods include passwords, biometrics, or security tokens. For instance, a fingerprint scan on a workstation ensures that only the authorized user can log in.  

2. **Authorization**: Determines what actions authenticated users can perform and which resources they can access. For example, a system might allow a database administrator to modify schemas but restrict regular users to viewing data only.  

3. **Accounting**: Tracks and logs user actions within a system, providing an audit trail for compliance and forensic purposes. Logs might include login attempts, file modifications, and access to restricted areas, ensuring accountability for all actions.  

Together, the AAA model provides a layered approach to secure access, combining verification, permission enforcement, and traceability.  

---

### **Know the difference between identification and authentication.**  

**Identification** is the process of claiming an identity, while **authentication** is the process of verifying that identity. Identification occurs when a user provides an identifier, such as a username, email, or ID card, to the system. Authentication follows by validating the identifier through credentials like passwords, biometric scans, or PINs.  

For example, when logging into a corporate network, entering a username identifies the user to the system, while providing a password authenticates their claim. Without successful authentication, the system cannot verify that the user is who they claim to be.  

This distinction is critical in designing access control systems, as identification alone does not guarantee legitimacy; authentication ensures trust in the claimed identity.  

---

### **Understand the establishment of identity, registration, and proofing.**  

Establishing identity involves verifying and documenting a user's identity through **registration** and **identity proofing** processes. During registration, the organization collects information such as government-issued IDs, biometric data, or other credentials. Identity proofing ensures that the provided information matches the individual.  

For example, a new employee might provide a passport and undergo biometric enrollment as part of onboarding. The HR system validates these credentials against trusted sources, such as government databases. Once proofing is complete, the employee is assigned a unique identifier in the organization's identity management system.  

This process ensures that all users are accurately identified, reducing the risks of impersonation, identity fraud, and unauthorized access.  

---

### **Understand the difference between authorization and accounting.**  

**Authorization** defines what actions an authenticated user can perform, while **accounting** tracks and records those actions. Authorization ensures that users access only the resources they are permitted to use, while accounting provides an audit trail for monitoring and analysis.  

For instance, after an employee logs into a system, authorization policies might restrict them to view-only access to sensitive files. Simultaneously, accounting logs record the files accessed and the time of access. If the user attempts unauthorized actions, these logs provide evidence for further investigation.  

By integrating authorization and accounting, organizations maintain control over resources while ensuring visibility and accountability for all user activities.  

---

### **Know the primary authentication factors.**  

Authentication factors are categorized into three primary types, often referred to as **something you know, something you have, and something you are**:  

1. **Something You Know**: Information such as passwords, PINs, or security questions. For example, a user entering a password to access their email is relying on this factor.  

2. **Something You Have**: Physical or digital objects like smart cards, hardware tokens, or mobile devices. An example is using a security token to generate a one-time password (OTP).  

3. **Something You Are**: Biometric attributes, such as fingerprints, facial recognition, or iris scans. For instance, unlocking a smartphone using facial recognition is an example of this factor.  

Using multiple factors, as in **multi-factor authentication (MFA)**, significantly enhances security by requiring attackers to compromise more than one method.  

---

### **Understand important authentication concepts.**  

Important authentication concepts include **multi-factor authentication (MFA)**, **passwordless authentication**, and **adaptive authentication**.  

- **MFA**: Combines two or more authentication factors, such as a password (knowledge) and a hardware token (possession), to strengthen security.  
- **Passwordless Authentication**: Relies on methods like biometrics or push notifications, eliminating the vulnerabilities associated with passwords.  
- **Adaptive Authentication**: Adjusts the level of authentication required based on risk factors, such as location or device reputation. For instance, a user logging in from an unfamiliar location may be required to answer additional security questions.  

These concepts ensure that authentication remains robust while balancing user convenience and security.  

---

### **Understand single sign-on.**  

**Single Sign-On (SSO)** allows users to access multiple systems or applications with one set of login credentials. By centralizing authentication, SSO improves user convenience and reduces the need for managing multiple passwords.  

For example, a user logging into a corporate SSO portal gains access to email, file storage, and CRM tools without needing to authenticate separately for each service. Technologies like **SAML**, **OAuth**, and **OpenID Connect** enable secure SSO implementations.  

SSO enhances security by reducing password fatigue and simplifying credential management, while also streamlining user access to organizational resources.  

---

### **Describe how federated identity systems are implemented.**  

Federated identity systems allow users to authenticate across multiple systems or organizations using a single set of credentials. These systems rely on trust relationships between **identity providers (IdPs)** and **service providers (SPs)**.  

For example, a user might log into a third-party cloud application using their corporate credentials. Protocols like **SAML** or **OpenID Connect** facilitate secure communication between the IdP and SP, enabling seamless access without requiring separate accounts.  

Federated identity simplifies authentication, improves user experience, and reduces the administrative burden of managing multiple identities across systems.  

---

### **Describe Just-in-Time (JIT) provisioning.**  

**Just-in-Time (JIT) provisioning** automatically creates and manages user accounts when they are needed, rather than pre-provisioning accounts in advance.  

For example, when a contractor logs into a project management tool for the first time, JIT provisioning dynamically creates their account based on predefined rules, such as role and project assignment. Once the contractor no longer requires access, the account is automatically deprovisioned.  

JIT provisioning reduces administrative overhead, minimizes unused accounts, and ensures that users only have access for the duration they need it, aligning with the principle of least privilege.  

---

### **Know about credential management systems.**  

Credential management systems, such as **password vaults** or **identity managers**, securely store and manage user credentials. These systems ensure that sensitive information, like passwords, is encrypted and accessible only to authorized users.  

For instance, a password vault might generate and store complex passwords for each application a user accesses, eliminating the need to remember them. Enterprise credential managers often integrate with SSO and MFA solutions, further enhancing security.  

By automating credential storage and management, these systems reduce the risk of password compromise and improve organizational security.  

---

### **Explain session management.**  

Session management involves controlling and securing user sessions to prevent unauthorized access or hijacking. Techniques include session timeouts, secure cookies, and monitoring for suspicious activity.  

For example, a web application might automatically log out a user after 15 minutes of inactivity. Secure cookies ensure that session data cannot be intercepted or manipulated. Additionally, systems might monitor for concurrent logins from multiple locations, which could indicate account compromise.  

Effective session management balances user convenience with robust security, ensuring that sessions remain secure throughout their lifecycle.  

---

### **Understand the identity and access provisioning lifecycle.**  

The **identity and access provisioning lifecycle** encompasses all stages of managing user access, from onboarding to offboarding.  

1. **Provisioning**: Granting users access to necessary resources during onboarding. For example, a new employee might receive access to email, file storage, and role-specific applications.  
2. **Review and Maintenance**: Periodically reviewing user permissions to ensure they remain aligned with job responsibilities.  
3. **Deprovisioning**: Revoking access when a user leaves the organization or changes roles, ensuring that no unauthorized access persists.  

By managing this lifecycle effectively, organizations minimize security risks and maintain compliance with access control policies.  

---

### **Explain the importance of group and role definition and transition.**  

Group and role definitions simplify access management by assigning permissions based on roles rather than individuals. This ensures consistency, reduces administrative overhead, and enforces the principle of least privilege.  

For example, an "HR Manager" role might include permissions to access payroll systems and personnel files. When an employee transitions to this role, assigning them to the group instantly grants appropriate permissions. Similarly, removing them from the group upon role transition revokes access.  

Regularly reviewing and updating role definitions ensures that they align with organizational needs and security policies, preventing privilege creep and unauthorized access.  

---

### **Describe the purpose of account access reviews.**  

Account access reviews periodically evaluate user permissions to ensure they align with current job responsibilities and security policies. These reviews identify inactive accounts, redundant permissions, or privilege escalation.  

For example, an access review might uncover a contractor account that remains active long after the project ended, prompting deprovisioning. Regular reviews also help organizations maintain compliance with regulations like **GDPR** or **SOX**.  

By conducting thorough access reviews, organizations reduce risks associated with insider threats, privilege abuse, and non-compliance.

# Chapter 14: Controlling and Monitoring Access  

---

## Domain 3.0: Security Architecture and Engineering  
## Domain 5.0: Identity and Access Management (IAM)  

---

### **Identify common authorization mechanisms.**  

Authorization mechanisms are systems and policies that determine what resources an authenticated user can access and what actions they can perform. These mechanisms play a critical role in securing resources and ensuring that access aligns with organizational policies. Common authorization mechanisms include:  

1. **Role-Based Access Control (RBAC)**: Grants permissions based on user roles, which are predefined according to organizational responsibilities. For example, an "Admin" role might have permission to modify configurations, while a "User" role can only view data.  

2. **Rule-Based Access Control**: Utilizes predefined rules or conditions to grant or deny access. For example, access might be restricted to specific hours or geographic locations.  

3. **Attribute-Based Access Control (ABAC)**: Evaluates attributes such as user identity, resource type, and environmental conditions (e.g., time or device) to make access decisions. For example, ABAC might allow access only if a user is in a certain department and using a company-issued device.  

4. **Mandatory Access Control (MAC)**: Enforces strict access policies based on classifications like "Confidential" or "Top Secret." Users can only access resources within their clearance level.  

5. **Discretionary Access Control (DAC)**: Allows resource owners to grant or revoke access permissions to other users. This model is flexible but can be prone to human error.  

These mechanisms ensure that access is tightly controlled, reducing the risk of unauthorized actions or data breaches.

---

### **Describe key concepts of the discretionary access control (DAC) model.**  

The **Discretionary Access Control (DAC)** model allows resource owners to control access to their resources. It is one of the most flexible and widely used access control models.  

**Key Concepts:**  

1. **Ownership**: In DAC, the owner of a resource (e.g., a file or database) determines who can access it and what permissions (read, write, execute) they have.  

2. **Delegation**: Owners can delegate access rights to other users. For example, a manager might share a report with a team member by granting them read access.  

3. **Flexibility and Simplicity**: DAC is straightforward to implement and allows users to manage access without involving administrators constantly.  

**Challenges:**  
While DAC offers flexibility, it can lead to security issues if owners grant permissions indiscriminately. It is also susceptible to insider threats, as unauthorized users may gain access through shared permissions.  

---

### **Describe key concepts of the role-based access control (RBAC) model.**  

**Role-Based Access Control (RBAC)** assigns permissions to users based on their roles within the organization, streamlining access management and improving security.  

**Key Concepts:**  

1. **Roles and Permissions**: Roles are defined based on job functions (e.g., "HR Manager," "IT Admin"), and permissions are assigned to these roles. Users inherit permissions when assigned a role.  

2. **Separation of Duties (SoD)**: RBAC enforces SoD by ensuring that critical tasks are divided among different roles. For example, a person creating invoices cannot also approve payments.  

3. **Scalability and Maintenance**: RBAC simplifies access management, especially in large organizations. Adding or removing users from roles automatically adjusts their permissions without needing individual updates.  

**Example:**  
An "HR Manager" role might include permissions to view and edit employee records. Assigning this role to a new manager instantly grants them access to the relevant systems.  

---

### **Describe key concepts of the rule-based access control model.**  

**Rule-Based Access Control** uses predefined rules to grant or deny access. These rules are often conditional, based on environmental factors or specific policies.  

**Key Concepts:**  

1. **Conditional Access**: Rules define when and how access is granted. For example, a user may only access a system during business hours or from within a specific IP range.  

2. **Dynamic Enforcement**: Access decisions are automatically enforced based on the evaluation of rules. For instance, a rule might allow database access only if the user's device has up-to-date antivirus software.  

3. **Centralized Management**: Rules are created and managed by administrators, ensuring consistency and reducing errors.  

Rule-based access control is often used in **firewalls**, **intrusion prevention systems**, and **cloud security policies**, where access is granted or denied based on predefined conditions.

---

### **Describe key concepts of the attribute-based access control (ABAC) model.**  

**Attribute-Based Access Control (ABAC)** evaluates multiple attributes to determine access rights, making it one of the most flexible and granular access control models.  

**Key Concepts:**  

1. **Attributes**: Attributes are characteristics of users, resources, or environments. Examples include user roles, device types, time of access, and sensitivity levels of data.  

2. **Policy-Based Rules**: Access is granted based on policies that evaluate a combination of attributes. For example, an ABAC policy might grant access if the user is in the "Finance Department," the resource is classified as "Public," and the request originates from a company device.  

3. **Granularity**: ABAC allows fine-grained access control, enabling organizations to define complex access policies that adapt to varying contexts.  

ABAC is particularly effective in dynamic environments, such as cloud computing, where traditional models may struggle to keep up with changing conditions.

---

### **Describe key concepts of the mandatory access control (MAC) model.**  

**Mandatory Access Control (MAC)** enforces strict access policies based on data classifications and user clearances, providing the highest level of security.  

**Key Concepts:**  

1. **Data Classification**: Resources are labeled with classifications like "Confidential," "Secret," or "Top Secret."  

2. **User Clearance**: Users are assigned clearance levels that determine the highest classification they can access.  

3. **Policy Enforcement**: Access decisions are enforced by the system, not the user. For example, a document marked "Confidential" can only be accessed by users with a "Confidential" or higher clearance.  

MAC is commonly used in government and military systems, where the protection of sensitive information is critical.  

---

### **Describe key concepts of the risk-based access control model.**  

**Risk-Based Access Control (RBAC)** dynamically adjusts access permissions based on the assessed risk associated with a request.  

**Key Concepts:**  

1. **Risk Assessment**: Evaluates factors such as device security, user location, and behavior anomalies. For example, a login attempt from an unfamiliar location might trigger additional authentication steps.  

2. **Adaptive Policies**: Access decisions adapt to the current risk level. High-risk scenarios may require multi-factor authentication or deny access altogether.  

3. **Behavior Analytics**: Monitors user behavior to detect anomalies. For instance, downloading a large volume of sensitive files in a short period might trigger access restrictions.  

Risk-based access control enhances security by continuously adapting to evolving threats.

---

### **Understand single sign-on methods used on the Internet.**  

**Single Sign-On (SSO)** allows users to access multiple systems or applications with a single authentication process, simplifying access management and improving user experience.  

**Methods Used on the Internet:**  

1. **SAML (Security Assertion Markup Language)**: Used in web-based SSO, enabling secure exchange of authentication data between identity providers (IdPs) and service providers (SPs).  

2. **OAuth and OpenID Connect**: Common in consumer applications, allowing users to log in using accounts from platforms like Google or Facebook.  

3. **Federated Identity**: Enables SSO across organizational boundaries, such as between a company and its cloud service provider.  

SSO reduces the need for multiple passwords, improving security and reducing the risk of credential compromise.

---

### **Describe Kerberos.**  

**Kerberos** is a network authentication protocol that uses tickets to securely authenticate users and services. It is widely used in enterprise environments for its ability to minimize credential exposure.  

**How It Works:**  

1. **Authentication**: The user logs in and receives a Ticket Granting Ticket (TGT) from the Key Distribution Center (KDC).  
2. **Service Request**: The user presents the TGT to the KDC to obtain a service ticket.  
3. **Resource Access**: The service ticket is used to authenticate the user to the requested resource.  

Kerberos reduces the need to transmit passwords over the network, mitigating the risk of interception.  

---

### **Understand the purpose of AAA protocols.**  

The **Authentication, Authorization, and Accounting (AAA)** protocols provide a framework for managing and securing access to resources.  

**Purpose:**  

1. **Authentication**: Verifies the identity of users, devices, or systems.  
2. **Authorization**: Determines what resources authenticated users can access and what actions they can perform.  
3. **Accounting**: Logs user activities to provide an audit trail for security and compliance purposes.  

AAA protocols, such as RADIUS and TACACS+, are commonly used in network environments to enforce consistent access control policies.  

---

### **Describe privilege escalation.**  

**Privilege escalation** occurs when a user or process gains unauthorized access to higher privileges, either maliciously or due to a system misconfiguration.  

**Types:**  

1. **Vertical Escalation**: Gaining administrative privileges from a lower-level account.  
2. **Horizontal Escalation**: Accessing another user's privileges without increasing privilege levels.  

Privilege escalation poses a significant risk, as it can lead to unauthorized access to sensitive data or critical systems. Mitigation strategies include limiting administrative privileges, auditing privilege usage, and using tools like **sudo** for controlled privilege elevation.  

---

### **Explain zero-trust principles.**  

The **Zero-Trust** model eliminates implicit trust within a network, requiring verification of all users and devices regardless of their location.  

**Principles:**  

1. **Least Privilege**: Grant users and devices only the minimum access needed.  
2. **Continuous Verification**: Continuously validate identity, device health, and context.  
3. **Micro-Segmentation**: Isolate network segments to prevent lateral movement.  

Zero-trust enhances security by assuming that breaches are inevitable and focusing on limiting potential damage.  

---

### **Know about Kerberos exploitation attacks.**  

Kerberos exploitation attacks target vulnerabilities in the Kerberos protocol.  

**Examples:**  

1. **Golden Ticket Attack**: Forging a Ticket Granting Ticket (TGT) to gain unlimited access across a domain.  
2. **Pass-the-Ticket**: Stealing service tickets to impersonate users without needing their credentials.  

Mitigation strategies include monitoring ticket usage, implementing strong encryption, and rotating encryption keys regularly.  

---

### **Know how brute-force and dictionary attacks work.**  

**Brute-Force Attacks** attempt every possible password combination until the correct one is found. **Dictionary Attacks** use precompiled lists of common passwords.  

Mitigation techniques include:  

1. **Account Lockouts**: Lock accounts after a certain number of failed login attempts.  
2. **MFA**: Add additional layers of authentication.  
3. **Password Policies**: Enforce strong passwords to reduce vulnerability.  

# Payment Card Industry Data Security Standard (PCI DSS)

# What is PCI DSS?

The **Payment Card Industry Data Security Standard (PCI DSS)** is a set of security requirements that organizations must follow when they **store, process, or transmit payment card information**.

Its primary goal is to:

- Protect cardholder data
- Prevent credit/debit card fraud
- Reduce data breaches
- Ensure secure payment transactions

- **Introduced:** 2004
- **Current Major Version:** PCI DSS 4.0.1
- **Applies Worldwide:** Yes

---

# Who Must Comply with PCI DSS?

PCI DSS applies to **any organization** that accepts, processes, stores, or transmits payment card information.

Examples include:

- Online stores (E-commerce)
- Retail stores
- Restaurants
- Hotels
- Banks
- Payment processors
- Healthcare organizations accepting card payments
- Cloud service providers handling payment data

### Example

> An online shopping website accepts Visa and Mastercard payments. It must comply with PCI DSS.

---

# What is Cardholder Data (CHD)?

**Cardholder Data (CHD)** includes information found on a payment card.

Examples:

- Cardholder name
- Primary Account Number (PAN)
- Expiration date
- Service code

### Example

> A website stores a customer's card number and expiration date to process future payments. This information is Cardholder Data.

---

# What is Sensitive Authentication Data (SAD)?

Sensitive Authentication Data includes information used to authenticate payment transactions.

Examples:

- CVV/CVC/CVV2 code
- PIN
- PIN Block
- Full magnetic stripe data
- EMV chip authentication data

> **Important:** Sensitive Authentication Data **must never be stored after authorization**, even if encrypted.

### Example

> An online store saves customers' CVV numbers after payment. This is a PCI DSS violation.

---

# PCI DSS Security Goals

PCI DSS aims to:

- Build secure networks
- Protect cardholder data
- Maintain vulnerability management
- Implement strong access control
- Monitor and test security
- Maintain an information security policy

### Example

> A retail company encrypts payment information and regularly updates its systems to prevent attacks.

---

# The 12 PCI DSS Requirements

PCI DSS is built around **12 core security requirements**.

## Goal 1: Build and Maintain a Secure Network

### 1. Install and Maintain Network Security Controls

- Use firewalls
- Secure network architecture
- Restrict unauthorized access

**Example**

> A company installs a firewall to block unauthorized internet traffic.

---

### 2. Apply Secure Configurations

- Change default passwords
- Disable unnecessary services
- Harden operating systems

**Example**

> A new payment server's default admin password is changed before deployment.

---

## Goal 2: Protect Account Data

### 3. Protect Stored Cardholder Data

Organizations should:

- Encrypt stored data
- Mask card numbers
- Store only necessary information

**Example**

> A database stores only the last four digits of a customer's card number.

---

### 4. Encrypt Data During Transmission

Cardholder data must be encrypted whenever it travels across public networks.

**Example**

> An online payment page uses HTTPS (TLS) to encrypt card details during checkout.

---

## Goal 3: Maintain a Vulnerability Management Program

### 5. Protect Systems Against Malware

Organizations should:

- Install antivirus software
- Keep malware protection updated
- Scan systems regularly

**Example**

> All employee computers run updated antivirus software.

---

### 6. Develop and Maintain Secure Systems

Organizations should:

- Apply security patches
- Fix vulnerabilities quickly
- Follow secure coding practices

**Example**

> A web application is updated immediately after a critical security vulnerability is discovered.

---

## Goal 4: Implement Strong Access Control Measures

### 7. Restrict Access to Cardholder Data

Access should be based on **business need-to-know**.

**Example**

> Customer service representatives cannot access payment databases.

---

### 8. Identify and Authenticate Users

Organizations should use:

- Unique user IDs
- Strong passwords
- Multi-factor Authentication (MFA)

**Example**

> Every administrator logs in using a unique account with MFA enabled.

---

### 9. Restrict Physical Access

Protect physical systems containing payment information.

Examples:

- Locked server rooms
- CCTV surveillance
- Access cards
- Visitor logs

**Example**

> Only authorized employees can enter the payment server room using ID badges.

---

## Goal 5: Regularly Monitor and Test Networks

### 10. Log and Monitor Access

Organizations should:

- Keep audit logs
- Monitor suspicious activity
- Review security logs regularly

**Example**

> Every login to the payment database is recorded and reviewed.

---

### 11. Test Security Regularly

Organizations should perform:

- Vulnerability scanning
- Penetration testing
- Security monitoring
- Network testing

**Example**

> A company hires ethical hackers to test the security of its payment application.

---

## Goal 6: Maintain an Information Security Policy

### 12. Maintain Security Policies

Organizations should:

- Create security policies
- Train employees
- Conduct risk assessments
- Review policies regularly

**Example**

> Employees complete annual cybersecurity awareness training.

---

# PCI DSS Levels

Organizations are classified into **four merchant levels** based on the number of card transactions processed annually.

| Level | Annual Transactions | Typical Requirement |
|--------|--------------------|---------------------|
| **Level 1** | Over 6 million | Annual on-site assessment by a Qualified Security Assessor (QSA) |
| **Level 2** | 1 million – 6 million | Self-Assessment Questionnaire (SAQ) or assessment |
| **Level 3** | 20,000 – 1 million (e-commerce) | SAQ and vulnerability scans |
| **Level 4** | Fewer than 20,000 e-commerce or up to 1 million total | SAQ and basic security validation |

### Example

> A small online store processing 10,000 online card transactions per year is generally considered a Level 4 merchant.

---

# Common PCI DSS Violations

Examples include:

- Storing CVV numbers
- Weak passwords
- Missing software updates
- No encryption
- Shared user accounts
- Lack of employee training
- No firewall protection
- Missing audit logs

### Example

> An organization stores customers' CVV codes in its database. This is a serious PCI DSS violation.

---

# Benefits of PCI DSS Compliance

Organizations benefit by:

- Reducing payment fraud
- Protecting customer information
- Improving cybersecurity
- Building customer trust
- Reducing financial losses
- Meeting payment processor requirements

### Example

> Customers are more confident purchasing from an online store that securely handles payment information.

---

# Penalties for Non-Compliance

Failure to comply with PCI DSS may result in:

- Financial penalties from payment brands or acquiring banks
- Increased transaction fees
- Mandatory forensic investigations after breaches
- Loss of the ability to process payment cards
- Legal and reputational damage

### Example

> A retailer suffers a payment card breach due to poor security controls. Its acquiring bank may impose fines and restrict its ability to accept card payments.

---

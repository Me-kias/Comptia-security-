# 🔐 AAA: Authentication, Authorization, Accounting

## **1. Authentication**
- Process of proving **who you are**.
- Common steps:
  1. **Identification** → Claim your identity (username, email, etc.)
  2. **Authentication** → Prove it (password, MFA, certificate)
  
### Example:
- Logging into a VPN:
  - Client sends username/password to VPN concentrator
  - VPN checks credentials with a central **AAA server**
  - Access granted if credentials are valid

### Device Authentication:
- Devices can authenticate using **digitally signed certificates**
- Certificates are issued and verified by a **Certificate Authority (CA)**
- Confirms the device is trusted without storing passwords locally

---

## **2. Authorization**
- Determines **what resources you can access** after authentication
- Scales better using **roles, groups, and attributes** instead of per-user permissions

### Example:
- Shipping & Receiving department:
  - Instead of assigning permissions individually, create a **Shipping & Receiving group**
  - Add all users in that department to the group
  - Group automatically gets access to relevant resources (shipping labels, customer data, reports, etc.)

---

## **3. Accounting**
- Logs actions and events for auditing purposes
- Example:
  - Login/logout times
  - Data transferred
  - Actions performed by users or devices

---

## **Scalable AAA Implementation**
1. Users authenticate → identity verified
2. Group/role-based authorization → access to resources
3. Accounting → logs activities for auditing

This **AAA framework** ensures secure access while simplifying management in large environments.

# Security Risk Assessment Report

> **Course:** Google Cybersecurity Certificate — Course 3: Connect and Protect: Networks and Network Security
> **Activity:** Security Risk Assessment
> **Author:** Armando Millauro
> **Date:** November 2026

---

## Scenario

A social media organization recently experienced a major data breach that compromised the safety of their customers' personal information, including names and addresses.

As a security analyst, I was tasked with inspecting the organization's network and recommending hardening practices to prevent future attacks.

### Vulnerabilities identified

| # | Vulnerability |
|---|---------------|
| 1 | Employees share passwords |
| 2 | The admin password for the database is set to the default |
| 3 | The firewalls do not have rules to filter inbound and outbound traffic |
| 4 | Multifactor authentication (MFA) is not used |

---

## Hardening methods selected

1. Password policies
2. Firewall rules and regular firewall maintenance (port filtering)
3. Multi-factor authentication (MFA)

---

## Recommendations

### 1. Password policies

Password policies set rules for how complex passwords must be, forbid sharing passwords between employees, and require changing default passwords, like the database administrator password. They also limit the number of failed login attempts, which helps stop brute force attacks. The policy is always active, and it should be reviewed regularly, for example every six months. When an employee leaves the company, their account should be disabled immediately.

### 2. Firewall rules and maintenance

Firewall rules decide which traffic can enter and leave the network. With port filtering, only the ports that are really needed stay open, and all the others are blocked. Outbound rules can also help stop stolen data from leaving the network. The rules work all the time, and they should be reviewed and updated regularly, and right away when a new threat appears.

### 3. Multi-factor authentication (MFA)

MFA asks users to confirm their identity with a second factor, such as a fingerprint or a code on their phone, in addition to the password. Even if an attacker steals or receives a shared password, they cannot log in without the second factor. This adds another layer of protection (defense in depth). MFA is always active, at every login.

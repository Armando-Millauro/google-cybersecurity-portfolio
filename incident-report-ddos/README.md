# Incident Report: DDoS Attack (ICMP Flood) – NIST CSF Analysis

Cybersecurity portfolio project from the **Google Cybersecurity Certificate**.

In this project I analyze a network security incident and build an improvement plan using the **NIST Cybersecurity Framework (CSF)** and its five core functions: Identify, Protect, Detect, Respond and Recover.

---

## Scenario

I work as a cybersecurity analyst for a multimedia company that offers web design, graphic design and social media marketing services to small businesses.

The company suffered a **DDoS attack** that took down the internal network for **two hours**:

- Network services suddenly stopped responding because of a **flood of incoming ICMP packets**.
- Normal internal traffic could not reach any network resources.
- The attacker got in through a **firewall that was not properly configured**.

---

## Incident Report

| NIST CSF function | Analysis |
|---|---|
| **Summary** | The company experienced a DDoS attack. Network services stopped responding for 2 hours due to a flood of incoming ICMP packets. The attacker got in through a firewall that was not properly configured. The team responded by blocking incoming ICMP packets, taking non-critical network services offline, and restoring critical network services. |
| **Identify** | A malicious actor targeted the company with an ICMP flood attack (DDoS). The entire internal network was affected. The attacker exploited an unconfigured firewall, which let the flood of ICMP packets reach the network. Critical network resources had to be secured and restored. |
| **Protect** | The network security team implemented a new firewall rule to limit the rate of incoming ICMP packets. They also enabled source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets. The team should also audit firewall configurations regularly and train IT staff so this kind of misconfiguration does not happen again. |
| **Detect** | The team installed network monitoring software to detect abnormal traffic patterns, such as a sudden spike in ICMP packets. They also set up an IDS/IPS system to filter out ICMP traffic based on suspicious characteristics and alert the security team. |
| **Respond** | The incident management team responded by blocking incoming ICMP packets, taking all non-critical network services offline, and restoring critical network services. The cybersecurity team then investigated the incident and found that the attacker used an unconfigured firewall. In the future, the team will isolate affected systems quickly and review network logs to find suspicious activity. |
| **Recover** | To recover from a DDoS attack, access to network services needs to be restored to a normal working state. In the future, external ICMP flood attacks can be blocked at the firewall. Then, all non-critical network services should be stopped to reduce internal network traffic. Next, critical network services should be restored first. Finally, once the flood of ICMP packets has timed out, all non-critical network systems and services can be brought back online. |

---

## Reflections

This incident showed how a single misconfigured firewall can take down an entire network. Simple measures like rate limiting, IP verification and continuous monitoring can prevent most ICMP flood attacks. Regular firewall audits should be part of the company's security routine.

---

## Skills shown

- Incident analysis and documentation
- Applying the NIST Cybersecurity Framework (CSF)
- Network security concepts: DDoS, ICMP flood, firewall rules, IP spoofing, IDS/IPS
- Writing clear security recommendations

---

*Author: Armando – Google Cybersecurity Certificate (Coursera)*

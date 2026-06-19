# Incident Report Analysis Using NIST CSF

# Project Overview and Scenario

As a cybersecurity analyst for a multimedia company offering web design and marketing solutions, I was tasked with analyzing a recent security incident. The organization's internal network was compromised for two hours due to a Distributed Denial of Service (DDoS) attack.

A malicious actor overwhelmed the network with an incoming flood of ICMP packets through an unconfigured firewall, causing all network services to stop responding. This report utilizes the **National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF)** to document the incident, analyze the response, and outline a strategic plan to improve the company's network security posture.

# 1. Summary

The company experienced a critical security event when all network services suddenly stopped responding. The cybersecurity team found the disruption was caused by a distributed denial of services (DDoS) attack through a flood of incoming ICMP packets. The team responded by blocking the attack and stopping all non-critical network services, so that critical network services could be restored and business continuity maintained.

# 2. Identify

**Threat Actor & Vector**: A malicious actor or actors targeted the company with an ICMP flood attack leveraging an unconfigured firewall vulnerability.

**Impact Scope**: The entire internal network was affected. Normal internal network traffic could not access any network resources.

**Asset Prioritization** All critical network resources needed to be secured and restored to a functioning state to minimize operational downtime.

# 3. Protect

To safeguard the organization's assets against similar vulnerabilities in the future, the cybersecurity team implemented the following proactive safeguards:

**Firewall Rules**: Implemented a new firewall rule to proactively limit the rate of incoming ICMP packets.

**Traffic Filtering**: Deployed an Intrusion Detection/Prevention System (IDS/IPS) to filter out and drop some ICMP traffic based on suspicious network characteristics.

# 4. Detect

To ensure continuous monitoring and rapid identification of future anomalies, the team improved detection capabilities by:

**Source Verification**: Configured source IP address verification on the firewall to check for and block spoofed IP addresses on incoming ICMP packets.

**Abnormal Traffic Monitoring**: Implemented advanced network monitoring software designed to detect abnormal traffic patterns and alert the team before a flood can overwhelm the network.

# 5. Respond

For future security events, the cybersecurity team has established a robust incident response protocol:

**Containment**: The team will immediately isolate affected systems to prevent further disruption to the network.

**Mitigation & Restoration**: They will attempt to restore any critical systems and services that were disrupted by the event based on priority.

**Forensic Analysis**: The team will analyze network logs to check for suspicious and abnormal activity.

**Communication**: The team will report all incidents to upper management and appropriate legal authorities, if applicable, ensuring full transparency.

# 6. Recover

To recover from a DDoS attack by ICMP flooding, access to network services needs to be restored to a normal functioning state securely and methodically:

**Immediate Blockage**: External ICMP flood attacks must first be blocked at the firewall.

**Traffic Reduction**: All non-critical network services should be stopped to reduce internal network traffic load.

**Prioritized Restoration**: Critical network services must be restored first.

**Full Recovery**: Finally, once the flood of ICMP packets has timed out and the threat is neutralized, all non-critical network systems and services can be safely brought back online.

Reflections & Notes

Applying the NIST Cybersecurity Framework (Identify, Protect, Detect, Respond, Recover) transitions an organization from a reactive security posture to a proactive and resilient one. By utilizing this framework, I was able to not only document the containment of a disruptive DDoS attack but also implement scalable defenses (like IDS/IPS and firewall rate limiting) that ensure the long-term integrity and availability of the company's digital infrastructure.

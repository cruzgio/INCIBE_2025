# INCIBE 2025 Incident Response Tools

## Server Analysis

### DeepBlueCLI
PowerShell Module for Threat Hunting via Windows Event Logs
* https://github.com/sans-blue-team/DeepBlueCLI
* https://youtu.be/G8XjSO_eshc?si=ifAX8PQS5Q80Xl2_

### Velociraptor
Velociraptor is a tool for collecting host-based state information using the Velociraptor Query Language (VQL) queries
* https://docs.velociraptor.app
* https://github.com/Velocidex/velociraptor
* https://docs.velociraptor.app/training/
* https://youtu.be/ie6-859ERv4?si=KJJrgaZKAHDQfs6c
* https://youtu.be/vB_rg0N69CY?si=Gaef--h3SeGnDk-T
 
### Sysinternals
Sysinternals Suite tools are valuable assets in incident response, offering insights into system behavior and facilitating the identification and analysis of security incidents. Tools like Process Monitor (Procmon) and Sysmon provide detailed logging of system events, enabling analysts to track process activity, network connections, and file system operations. 
* https://learn.microsoft.com/en-us/sysinternals/downloads/sysinternals-suite
* https://youtu.be/zIwUBTGjbws?si=0SxZ4VG3Qi0N5R9C

## Security Information and Event Management (SIEM) Log Analysis

### Security Onion
A free and open platform for threat hunting, network security monitoring, and log management. Security Onion includes best-of-breed free and open tools, including Suricata, Zeek, the Elastic Stack, and many others.
* https://securityonionsolutions.com
* https://securityonionsolutions.com/training#free-training

### Wazuh
Unified XDR and SIEM protection for endpoints and cloud workloads.
* https://wazuh.com
* https://youtu.be/dwr-4CXtOso?si=wUWQi-6dvUyo6Kt5
* https://youtu.be/nSOqU1iX5oQ?si=j_5NJ8TePdBN38SH

### JPCert Tool Analysis Result Sheet
The site summarizes the results of examining logs recorded in Windows upon execution of the 49 tools, which are likely to be used by the attacker who has infiltrated a network.
* https://jpcertcc.github.io/ToolAnalysisResultSheet

## Firewall Log Review

### Graylog
Graylog Open is a self-managed, SSPL-licensed centralized log management solution designed for log data aggregation, analysis, and management.
* https://graylog.org/products/source-available/
* https://graylog.org/downloads/
* https://youtu.be/rDSjD_IBdy8?si=0Bk9dRdsjbBO__UL

### Elastic Stack -> OpenSearch
OpenSearch is an open-source, enterprise-grade search and observability suite that brings order to unstructured data at scale.
* https://opensearch.org
* https://opensearch.org/platform/security-analytics/
* https://docs.opensearch.org/docs/latest/security-analytics/
* https://docs.opensearch.org/docs/latest/security-analytics/sec-analytics-config/index/
* https://github.com/opensearch-project/security-analytics
* https://youtu.be/sO4nDnTVCfk?si=j_hGlayTOjw0U4u5
* https://youtu.be/c6sbQ6cmN0s?si=qqBRvQ4es9WB5fw5

### Kiwi Syslog Server
On-premises software to manage syslog messages, SNMP traps, and Windows event logs.
* https://www.solarwinds.com/free-tools/kiwi-free-syslog-server
* https://www.solarwinds.com/resources/video/kiwi-syslog-server-guided-tour

## Network Threat Hunting

### Real Intelligence Threat Analytics RITA
Open-source framework for detecting command and control communication through network traffic analysis. The RITA framework ingests Zeek logs in TSV or JSON format, or PCAPs converted to Zeek logs for analysis.
* https://www.activecountermeasures.com/free-tools/rita/
* https://www.activecountermeasures.com/ritav5-the-video-series/

### AC-Hunter
AC-Hunter is a software solution that continuously threat hunts your network to identify which of your systems have been compromised.
* https://www.activecountermeasures.com/ac-hunter-community-edition/
* https://youtu.be/t-9pcKzuuwc?si=HUzGWBLOPKicIJfW
* https://youtu.be/26saE26aQ4o?si=Tl0H5b3lVN9RTli6

### espy
Espy collects network traffic from Windows systems regardless of geographical location. The network traffic is then stored as Zeek logs on a server of your choosing. The traffic can also be forwarded to an Elasticsearch instance.
* https://www.activecountermeasures.com/free-tools/espy/
* https://github.com/activecm/espy
* https://youtu.be/voHyY2-qzno?si=24qazDRvjRoHleBt

## Active Defense and Cyber Deception

### Canary Tokens
Canarytokens is a free tool that helps you discover you've been breached by having attackers announce themselves.
* https://docs.canarytokens.org/guide/#what-are-canarytokens
* https://canarytokens.org/nest/
* https://youtu.be/K_TagJ4iRZU?si=j1wMo1BFKPM3oErK

### HoneyBadger
HoneyBadger is a framework for targeted geolocation. While honeypots are traditionally used to passively detect malicious actors, HoneyBadger is an Active Defense tool to determine who the malicious actor is and where they are located.
* https://github.com/adhdproject/honeybadger
* https://youtu.be/7LXfBSuaFFE?si=hU-AKqXA5KvetuDi

### Active Defense Harbinger Distribution (ADHD)
A suite of tools encompassing the active defense theme.
* https://github.com/adhdproject
* https://adhdproject.github.io/#!index.md

### MITRE Engage
MITRE Engage is a framework for planning and discussing adversary engagement operations that empowers you to engage your adversaries and achieve your cybersecurity goals.
* https://engage.mitre.org

## Endpoint Security Protection Analysis

### Elastic Security
SIEM and endpoint security solution from Elastic.
* https://www.elastic.co/security
* https://www.elastic.co/blog/continued-leadership-in-open-and-transparent-security

### OpenEDR
OpenEDR is an open-source endpoint detection and response platform that provides analytic detection with MITRE ATT&CK visibility for event correlation and root cause analysis of adversarial cyber threat activity and behaviors in real time.
* https://www.openedr.com
* https://github.com/ComodoSecurity/openedr
* https://youtu.be/MI5DMKuxhH0?si=NJO4iFzPWPR1E453

### OSSEC
OSSEC Community is the most basic version of the tool for hobbyists and do-it-yourselfers. You can tailor the free rules through OSSEC’s configuration options, adding custom alert rules and writing scripts to take action when alerts occur. 
* https://www.ossec.net/ossec-downloads/
* https://youtu.be/7c8xowHz0Ko?si=Li3Lz8On7698nkYV

## User and Entity Behavior Analytics (UEBA)

### Logon Tracer
LogonTracer is a tool for investigating malicious logons by visualizing and analyzing Windows Active Directory event logs.
* https://github.com/JPCERTCC/LogonTracer
* https://github.com/jpcertcc/logontracer/wiki
* https://youtu.be/aX-vTd7-moY?si=-cWdvDs9OnW1GQel

### OpenUBA
An open source user behavior analytics platform powered by the scientific computing ecosystem
* https://github.com/GACWR/OpenUBA
* https://openuba.org

### Hayasuba
Hayabusa is a Windows event log fast forensics timeline generator and threat hunting tool created by the Yamato Security group in Japan.
* https://github.com/Yamato-Security/hayabusa
* https://youtu.be/HXNAnxADRGE?si=p7plzmfOl1TgLmFW

## Endpoint Analysis

### Incident Response Cheat Sheets
SANS provides various IR cheat sheets.
* https://www.sans.org/posters/?focus-area=digital-forensics

### osquery
Osquery uses basic SQL commands to leverage a relational data-model to describe a device.
* https://osquery.io
* https://osquery.readthedocs.io/en/stable/
* https://github.com/osquery/osquery
* https://youtu.be/YpmGZseJbJY?si=BPZSCAKKr3eL-Alg

## Memory Analysis

### Volatility 
The Volatility Framework is a comprehensive, open-source collection of tools, implemented in Python under the GNU General Public License, for extracting digital artifacts from volatile memory (RAM) samples.
* https://volatilityfoundation.org
* https://github.com/volatilityfoundation/volatility
* https://youtu.be/2S_pi9qnIo8?si=4Q5k0eAhjBhR_GvO

## Cloud Event Log Analysis

### Falco
Falco is a cloud native security tool that provides runtime security across hosts, containers, Kubernetes, and cloud environments.
* https://falco.org
* https://falco.org/docs/
* https://youtu.be/0tBSKRvH3xo?si=YfHfboivXtczwf8N

### Hawk
Hawk is a web interface for Pacemaker HA clusters. Use it to configure, manage, and monitor just about any kind of application running in Linux as a cluster resource.
* https://github.com/ClusterLabs/hawk
* https://hawk-ui.github.io

### Permissions Audit

## BloodHoud
BloodHound uses graph theory to reveal the hidden and often unintended relationships within an Active Directory or Azure environment.
* https://github.com/SpecterOps/BloodHound
* https://bloodhound.specterops.io/get-started/quickstart/community-edition-quickstart
* https://bloodhound.specterops.io/home
* https://youtu.be/Iw1KjpzlvaI?si=rghIaI4u7zq-X-BB

## ScoutSuite
Scout Suite is an open source multi-cloud security-auditing tool that enables security posture assessment of cloud environments.
* https://github.com/nccgroup/ScoutSuite
* https://youtu.be/G3MDJSMvnRo?si=lL5_B_H6YVtD9IUo

## Prowler
Prowler is an open-source security tool designed to assess and enforce security best practices across AWS, Azure, Google Cloud, and Kubernetes. It supports tasks such as security audits, incident response, continuous monitoring, system hardening, forensic readiness, and remediation processes.
* https://github.com/prowler-cloud/prowler
* https://prowler.com
* https://docs.prowler.com/projects/prowler-open-source/en/latest/#prowler-app-installation
* https://youtu.be/FpdqG3Cy6ow?si=DFczNYzL6xzPTfwD


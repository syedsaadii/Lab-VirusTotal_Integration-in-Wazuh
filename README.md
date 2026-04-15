# 🛡️ Mini SOC Lab - Wazuh + VirusTotal

> A $0, open-source SIEM lab that automatically detects real malware in under 10 seconds.

**Built by:** [Syed Saad](https://www.linkedin.com/in/syedsaadii)

### Live Demo
<img width="399" height="81" alt="virus toatl" src="https://github.com/user-attachments/assets/4ad92ffa-3fe3-4a64-b7de-b51d412a32ca" />

### What It Does
✅ Real-time File Integrity Monitoring (FIM)
✅ Automatic hash lookup via VirusTotal API
✅ Custom Rule (100100) triggers Level 12 Critical Alert
✅ Full Threat Hunting dashboard in Wazuh

### Architecture
`[Wazuh Agent] -> [Wazuh Manager] -> [VirusTotal API] -> [Custom Alert Rule] -> [Dashboard]`

### 🚀 Setup in 5 Minutes
1. Install Wazuh Manager & Agent
2. Get free VirusTotal API key
3. Paste `configs/ossec.conf-snippet.xml` into `/var/ossec/etc/ossec.conf`
4. Paste `configs/local_rules.xml` into `/var/ossec/etc/rules/local_rules.xml`
5. Restart Wazuh: `systemctl restart wazuh-manager`
6. Test with EICAR file: `echo 'X5O!P%@AP[4\PZX54(P^)7CC)7}$EICAR...' > /tmp/test.txt`

### Tools Used
Wazuh SIEM | VirusTotal | Ubuntu | MITRE ATT&CK

⭐ Star this repo if it helped you land a SOC interview!

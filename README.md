
---

## 🏗️ Methodology
The assessment was performed in the following phases:

1. **Lab Setup**
   - Attacker Machine: Kali Linux
   - Target Machine: Windows 7 VM
   - Network: Isolated host-only environment

2. **Reconnaissance**
   - Nmap scanning for open ports and services
   - Service enumeration for SMB, RDP, RPC, HTTP

3. **Vulnerability Analysis**
   - Identified legacy protocols and misconfigurations
   - Documented risks and security gaps

4. **(Safe) Exploitation Scenarios**
   - *Theoretical discussion* of potential attack vectors  
   - Example: SMB enumeration, RDP brute-force risks, RPC service abuse  
   - Screenshots of scans included in `/docs/`

5. **Mitigation & Hardening**
   - Disable unused services
   - Apply latest security patches
   - Use strong credentials and account lockout policies
   - Restrict network access via firewall

---

## 🔑 Key Services Assessed
- **SMB (Port 445)** → Checked for SMBv1 & anonymous access
- **RDP (Port 3389)** → Assessed brute-force risk
- **RPC (Port 135)** → Reviewed exposure risk
- **HTTP (Port 80)** → Checked for default IIS misconfigurations

---

## 🛡️ Defensive Recommendations
- Upgrade legacy OS (Windows 7 → Windows 10/11 or Linux)
- Disable SMBv1 and enforce SMBv2+
- Use Network Level Authentication (NLA) for RDP
- Apply least-privilege principle
- Regular vulnerability scanning & patching

---

## 📚 References
- Nmap Security Scanner – https://nmap.org  
- Microsoft Windows 7 Security Lifecycle – https://learn.microsoft.com  
- CWE Common Weakness Enumeration – https://cwe.mitre.org  
- CVE Details – https://cvedetails.com  

---

✍️ **Author:** Isanka Sandaruwan Jayasundara  
🎓 **Project:** University Student Report – Vulnerability Assessment & Penetration Testing (Educational Only)  

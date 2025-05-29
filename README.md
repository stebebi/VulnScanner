# 🛡️ VulnScanner

**VulnScanner** is a PowerShell-based vulnerability scanning tool for Windows systems. It performs local and remote audits, identifies missing patches, outdated software, known CVEs, and common misconfigurations. All results are saved as structured CSV reports in a timestamped folder.

---

## 🔍 Features

- **Missing Patch Detection**  
  Identifies uninstalled security updates using Windows Update APIs.

- **Installed Software & CVE Lookup**  
  Enumerates installed applications and checks for known CVEs via the NIST NVD API.

- **Misconfiguration Checks**  
  Flags insecure system settings such as:
  - SMBv1 enabled
  - RDP status
  - Legacy TLS protocol usage

- **Remote Hotfix Validation**  
  Connects to remote hosts (via WinRM) to enumerate installed hotfixes.

- **Reporting**  
  All results are exported to `.csv` files, grouped in a timestamped output folder.

---

## 📁 Output Structure


---

## 💻 Usage

```powershell
# Run from PowerShell as Administrator
.\VulnScanner.ps1

🧩 Requirements
PowerShell 5.1+

Internet connection (for CVE API lookup)

Admin privileges (for full scan capabilities)

Scripts written to aid automated scanning during whitebox security/vuln assessments

# Poc's
### Invoke-WinEnum.ps1
	Invoke-WinEnum		-  Check Windows host security (thx to Harmj0y, lkys37en, and A-mIn3)
* General System Information
* Local users in Administrators, RDP, DCOM, PSRemote group
* Firewall, AntiVirus, and Spyware Product for Workstations
* Autologon Credentials
* Cached GPP Password
* Unattended Install Files
* Unquoted Services Paths
* AlwaysInstallElevated
* UAC Configuration 
* ACL on Local SMB Shares
* ACL on Service Binaries and Directories
* ACL on Possible High Privileged Scheduled Tasks Binaries and Directories
* ACL on AutoRuns Binaries and Directories for System and Local Administrators
* ACL on Directories located in System and Local Administrators PATH Variable
* Active Listenings Ports
* Installed Software
* Print Spool and Wpad Status
* PowerShell Logging
* LAPS
* Lsass Protection
* SMBv1
* PowerShell v2
* .Net Versions
* Windows Defender Configuration for Servers
* IIS (encrypted web.config strings, encrypted application pools and virtual directory passwords)
* MSSQL (Links, Users, Default and Weak Passwords, Databases, ACL on .mdf, Vulnerable configurations...)

(ACL's for System, Local Administrators, and TrustedInstaller is being ignored)
### SecurityAssessment.ps1
	Invoke-LinuxSSH		  -  Run Bash script on multiple hosts simultaneously with Posh-SSH
	Invoke-WindowsWMI	  -  Run PowerShell script on multiple hosts simultaneously with WMI
	Invoke-WindowsPS	  -  Run PowerShell script on multiple hosts simultaneously with PSRemote
	Get-RemoteCertificates	  -  Download all CA and Root Certificates from a remote host using OpenRemoteBaseKey
	Get-DomainCertificates	  -  Download all published CA, Root and CRL certificates
	Get-DomainExchangeVersion -  Get exchange version from ADSI and check if vuln to privexchange
	Invoke-NetEnum		  -  Mostly C# scripts from pingcastle (thx vletoux)
	Invoke-DomainEnum	  -  Runs simple checks on the domain
* Domain and Forest Trust
* CPassword in Sysvol
* Active Directory Integrated DNS Wildcard Record
* Password Policy
* MachineAccountQuota
* Get-DomainExchangeVersion
* Get-DomainCertificates
* Null and anonymous SMB login on DCs
* BloodHound
### bloodhoundanalytics.py
	Gather Active Directory statistics from BloodHound data
# Software

https://docs.microsoft.com/en-us/windows/security/threat-protection/security-compliance-toolkit-10

https://github.com/CISOfy/lynis

https://github.com/DenizParlak/Zeus

https://github.com/BloodHoundAD/BloodHound/

https://www.tenable.com/products/nessus

https://github.com/torrentalle/Ubuntu1804-CIS

https://github.com/dev-sec/windows-baseline

# Nessus Audit Files
https://github.com/nsacyber/Windows-Secure-Host-Baseline/tree/master/Windows/Compliance

https://github.com/nsacyber/Windows-Secure-Host-Baseline/tree/master/Windows%20Firewall/Compliance

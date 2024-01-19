# Windows-Administration-and-Hardening


I successfully completed this assignment, building on Group Policy Objectives and PowerShell fundamentals. Utilizing the Windows Server and Windows 10 machines in my Azure Windows RDP Host setup, I addressed tasks such as disabling Local Link Multicast Name Resolution (LLMNR) and implementing an account lockout policy on the Windows workstation. Additionally, I created a Group Policy Object enabling verbose PowerShell logging and transcription. I successfully crafted a PowerShell script to enumerate Access Control Lists and verified the PowerShell logging GPO's functionality by running the script and confirming logs in the designated directory. 

This comprehensive assignment enhanced my skills in Windows system administration and cybersecurity practices.


**Task 1: GPO - Disable LLMNR**
- Created "No LLMNR" GPO.
- Disabled "Turn Off Multicast Name Resolution" under Computer Configuration\Policies\Administrative Templates\Network\DNS Client.
- Linked GPO to GC Computers OU.

**Task 2: GPO - Account Lockout**
- Created "Account Lockout" GPO.
- Configured a reasonable account lockout policy for Windows 10.
- Linked GPO to GC Computers OU.

**Task 3: GPO - PowerShell Logging**
- Created "PowerShell Logging" GPO.
- Enabled module logging, PowerShell script block logging, script execution, and transcription.
- Linked GPO to GC Computers OU.

**Task 4: Script - Enumerate ACLs**
- Created "enum_acls.ps1" PowerShell script.
- Enumerated Access Control Lists for files/subdirectories within the current directory.

**Task 5: Verify PowerShell Logging GPO**
- Tested PowerShell logging GPO functionality.
- Ran `gpupdate`, launched PowerShell, navigated to C:\Windows, ran "enum_acls.ps1," and checked C:\Users\sysadmin\Documents for logs. GPO confirmed operational.

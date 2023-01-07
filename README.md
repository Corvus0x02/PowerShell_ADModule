# Background & Overview
This repository simply hosts a copy of Microsoft's signed ActiveDirectory PowerShell module and associated files. Active Directory (AD) is a directory service developed by Microsoft used to manage Windows networks. [Microsoft provides a nice overview](https://learn.microsoft.com/en-us/powershell/module/activedirectory/?view=windowsserver2022-ps) of the module on their website "*The Active Directory module for Windows PowerShell is a PowerShell module that consolidates a group of cmdlets. You can use these cmdlets to manage your Active Directory domains, Active Directory Lightweight Directory Services (AD LDS) configuration sets, and Active Directory Database Mounting Tool instances in a single, self-contained package.*"

One key point that is not mentioned however - ***When authenticated to a domain, a user has read access to all objects in that domain.*** This module therefore can be used for a number of use cases for non-network administrators like penetration testers, red teamers, and IT auditors for querying/enumerating information within an AD environment (domain users, group memberships, password policies, etc.) By using a built-in Microsoft tool, pentesters/red teamers are less likely to be detected and IT auditors have a tool that is better suited for their use cases. 

# Install & Setup
Recommended install/setup is to install Microsoft's Remote Server Administration Tools (RSAT). See [4SYSOPS Website](https://4sysops.com/wiki/how-to-install-the-powershell-active-directory-module/) for instructions. The primary DLL is typically saved at C:\Windows\Microsoft.NET\assembly\GAC_64\Microsoft.ActiveDirectory.Management and the rest of the module files are saved to C:\Windows\System32\WindowsPowerShell\v1.0\Modules\ActiveDirectory\

Alternatively, you can download and save Microsoft.ActiveDirectory.Management.dll from this repo and manually import it into a PowerShell instance by running "Import-Module .\Microsoft.ActiveDirectory.Management.dll" (not recommended unless you are in a lab environment.)

# Usage & Commands
[GitBook Command References](https://book.krobotsecurity.com/infosec/powershell-and-active-directory/active-directory-powershell-module)

# Additional References
[Nikhil "SamratAshok" Mittal's 2018 Blog Post](https://www.labofapenetrationtester.com/2018/10/domain-enumeration-from-PowerShell-CLM.html)

[The Cyber Mentor's Building an AD Lab](https://www.youtube.com/watch?v=xftEuVQ7kY0&ab_channel=TheCyberMentor)

[Building Free Active Directory Lab in Azure](https://kamran-bilgrami.medium.com/ethical-hacking-lessons-building-free-active-directory-lab-in-azure-6c67a7eddd7f)

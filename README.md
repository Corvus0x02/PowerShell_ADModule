# Background & Overview
Active Directory (AD) is a directory service developed by Microsoft used to manage Windows networks. [Microsoft provides a nice overview](https://learn.microsoft.com/en-us/powershell/module/activedirectory/?view=windowsserver2022-ps) of the PowerShell ActiveDirectory Module on their website "*The Active Directory module for Windows PowerShell is a PowerShell module that consolidates a group of cmdlets. You can use these cmdlets to manage your Active Directory domains, Active Directory Lightweight Directory Services (AD LDS) configuration sets, and Active Directory Database Mounting Tool instances in a single, self-contained package.*"

One key point that is not mentioned however - ***When authenticated to a domain, a user has read access to all objects in that domain.*** This module therefore can be used for a number of use cases for penetration testers, red teamers, and IT auditors for querying/enumerating information about an AD environment. By using a built-in Microsoft tool, pentesters/red teamers are less likely to be detected compared to using SharpHound, PowerView, etc. and IT auditors have a tool that is better suited for their use cases rather than leveraging "hacking tools" that provide similar capabilities. 

# File Information




A copy of Microsoft's signed ActiveDirectory PowerShell module and associated files.

Microsoft signed DLL for the ActiveDirectory PowerShell module
Just a backup for the Microsoft's ActiveDirectory PowerShell module from Server 2016 with RSAT and module installed. The DLL is usually found at this path: C:\Windows\Microsoft.NET\assembly\GAC_64\Microsoft.ActiveDirectory.Management
and the rest of the module files at this path: C:\Windows\System32\WindowsPowerShell\v1.0\Modules\ActiveDirectory\![image](https://user-images.githubusercontent.com/89099422/211167255-e546d56e-a835-48e6-a65d-a8eaf15be5aa.png)

Once imported


# Usage
Understand the Active Directory environment (number of forests, domains, domain trusts, etc.)
Install 
One-line commands can be found


# MD5 Hashes


# Additional References and Credit
https://github.com/samratashok/ADModule
https://www.labofapenetrationtester.com/2018/10/domain-enumeration-from-PowerShell-CLM.html
https://4sysops.com/wiki/how-to-install-the-powershell-active-directory-module/
https://learn.microsoft.com/en-us/powershell/module/activedirectory/?view=windowsserver2022-ps
[The Cyber Mentor](https://www.youtube.com/watch?v=xftEuVQ7kY0&ab_channel=TheCyberMentor)
[Building Free Active Directory Lab in Azure](https://kamran-bilgrami.medium.com/ethical-hacking-lessons-building-free-active-directory-lab-in-azure-6c67a7eddd7f)

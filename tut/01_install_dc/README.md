#01 Instaling the Domain Controller

1. Use 'sconfig' to
- change the hostname
- change the ip address to static
- change the dns server to your own ip address

2. Install the Active Directory Windows Feature

In PowerShell use command
Install-WindowsFeature AD-Domain-Services -IncludeManagement

Get-NetIPAddress

#Joining the domain through the Workstation

Add-Computer -Domainname xyz.com -Credential xyz\Administrator -Force -Restart

Make sure when using Terminal it is running in Administrator Mode.

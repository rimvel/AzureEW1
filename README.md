# AzureEW1

Azure Edu Workshop #1

# 1 Prerequisites:

- Azure Powershell (https://docs.microsoft.com/en-us/powershell/azure/install-azurerm-ps?view=azurermps-5.7.0)

Run Powershell as Administrator:
```powershell
Install-Module PowerShellGet -Force
Install-Module -Name AzureRM -AllowClobber

Import-Module -Name AzureRM
```

- Git (https://git-scm.com/download/win)

[64-bit](https://github.com/git-for-windows/git/releases/download/v2.16.2.windows.1/Git-2.16.2-64-bit.exe),
[32-bit](https://github.com/git-for-windows/git/releases/download/v2.16.2.windows.1/Git-2.16.2-32-bit.exe)

# 2 Description

- A
- B
- C


# Let's do it!

## Clone repository
Ensure you have Git for Windows installed.
Open a PowerShell console and type the following:

``` powershell
git clone https://github.com/rimvel/xxx.git c:\xxx\
Set-Location c:\xxx\step1\
```
![git-clone-repository][git-clone-repository]

## Login to Azure Powershell
Still in the PowerShell console, type the following:

``` powerhell
Login-AzureRmAccount
```

Enter your credentials
Select the desired subscription using:

``` powershell
Get-AzureRmSubscription

Set-AzureRmContext -Subscription 'MySubscriptionName'
```

Invoke the provisioning by typing:

``` powershell
& .\Invoke-Provisioning.ps1
```

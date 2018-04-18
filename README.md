# AzureEW1

Azure Edu Workshop #1

# Prerequisites:

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

# Description

- A
- B
- C


# Requirements
* [Azure PowerShell Module version 5.xx](https://github.com/Azure/azure-powershell/releases/tag/v5.2.0-January2018)
* [Git for Windows](https://git-scm.com/download/win)

In an Administrator PowerShell console window, type:

``` powershell
Install-Module -Name AzureRM -RequiredVersion 5.2.0 -Force
```

# Let's code!
## Clone repository
Ensure you have Git for Windows installed.

Open a PowerShell console and type the following:

``` powershell
git clone https://github.com/rimvel/GlobalAzureBootcamp2018.git c:\gab2018\

Set-Location c:\gab2018\step1\
```
![git-clone-repository][git-clone-repository]

## Provision OMS
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

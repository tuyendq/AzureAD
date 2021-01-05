# AzureAD


Get MFA list
```powershell
$today = Get-Date -Format yyyyMMdd
Connect-MsolService
Get-MsolUser | select DisplayName -ExpandProperty StrongAuthenticationUserDetails | ft DisplayName, PhoneNumber, Email
```

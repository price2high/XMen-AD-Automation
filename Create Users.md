```
Import-Module ActiveDirectory
$users = Import-Csv "C:\path\to\xmen_users.csv"

foreach ($user in $users) {
    $name = "$($user.FirstName) $($user.LastName)"
    $username = $user.Username
    $password = ConvertTo-SecureString "P@ssw0rd123" -AsPlainText -Force

    New-ADUser -Name $name `
               -GivenName $user.FirstName `
               -Surname $user.LastName `
               -SamAccountName $username `
               -UserPrincipalName "$username@yourdomain.com" `
               -AccountPassword $password `
               -Enabled $true `
               -Path "OU=XMen,DC=yourdomain,DC=com"

    Write-Host "Created user: $username"
}
```

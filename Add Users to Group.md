Import-Module ActiveDirectory
$users = Import-Csv "C:\path\to\xmen_users.csv"
$groupName = "XMenTeam"

foreach ($user in $users) {
    Add-ADGroupMember -Identity $groupName -Members $user.Username
    Write-Host "Added $($user.Username) to $groupName"
}

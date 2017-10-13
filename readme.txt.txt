Get-WmiObject -Class Win32_Desktop -ComputerName . ile bilgisayarýn adýný buldu.
Get-WmiObject -Class Win32_BIOS -ComputerName . BIOS bilgilerini listeledi.
Get-WmiObject -Class Win32_Processor -ComputerName . | Select-Object -Property [a-z]* Sistem bilgisi buldu.
"Write-Output">>powershell.txt iþletim sistemi sürüm bilgisi buldu.
Netstat -a ile Tüm TCP ve UDP baðlantýlarý ekrana bastý.
netstat -r ile IP yönlendirme tablosunun içeriðini görüntüledi.
Get-WmiObject -Class Win32_OperatingSystem -ComputerName . | Select-Object -Property BuildNumber,BuildType,OSType,ServicePackMajorVersion,ServicePackMinorVersion ile iþletim sistemi sürüm bilgisini buldu.

Get-WmiObject -Class Win32_OperatingSystem -ComputerName . | Select-Object -Property NumberOfLicensedUsers,NumberOfUsers,RegisteredUser ile kullanýcýlarý buldu.

Get-WmiObject -Class Win32_LogonSession -ComputerName . ile oturum bilgilerini buldu.

Get-WmiObject –Class win32_computersystem ile domain,ram miktarý,üretici firma gibi bilgileri buldu.
schtasks | Where-Object { $_ -Match "Ready*" -or $_ -Match "Running*"}  schedule tasklarý bulma.
Get-wmiobject win32_group ile grup info buldu.
Get-ADDomainController ile DC info buldu.






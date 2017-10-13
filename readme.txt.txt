Get-WmiObject -Class Win32_Desktop -ComputerName . ile bilgisayar�n ad�n� buldu.
Get-WmiObject -Class Win32_BIOS -ComputerName . BIOS bilgilerini listeledi.
Get-WmiObject -Class Win32_Processor -ComputerName . | Select-Object -Property [a-z]* Sistem bilgisi buldu.
"Write-Output">>powershell.txt i�letim sistemi s�r�m bilgisi buldu.
Netstat -a ile T�m TCP ve UDP ba�lant�lar� ekrana bast�.
netstat -r ile IP y�nlendirme tablosunun i�eri�ini g�r�nt�ledi.
Get-WmiObject -Class Win32_OperatingSystem -ComputerName . | Select-Object -Property BuildNumber,BuildType,OSType,ServicePackMajorVersion,ServicePackMinorVersion ile i�letim sistemi s�r�m bilgisini buldu.

Get-WmiObject -Class Win32_OperatingSystem -ComputerName . | Select-Object -Property NumberOfLicensedUsers,NumberOfUsers,RegisteredUser ile kullan�c�lar� buldu.

Get-WmiObject -Class Win32_LogonSession -ComputerName . ile oturum bilgilerini buldu.

Get-WmiObject �Class win32_computersystem ile domain,ram miktar�,�retici firma gibi bilgileri buldu.
schtasks | Where-Object { $_ -Match "Ready*" -or $_ -Match "Running*"}  schedule tasklar� bulma.
Get-wmiobject win32_group ile grup info buldu.
Get-ADDomainController ile DC info buldu.






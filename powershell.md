# Backup Drivers

Export-WindowsDriver -Online -Destination c:\Temp\Driver
  
# Wi-Fi password on your computer

Netsh WLAN show profile name=”lan_name” key=clear

# Vedere dettagli scheda madre

wmic baseboard get product,Manufacturer,version,serialnumber

# Vedere dettagli disco installato

Get-PhysicalDisk | Format-Table -AutoSize

# Trovare product key Windows 10

(Get-WmiObject -query ‘select * from SoftwareLicensingService’).OA3xOriginalProductKey

# rewire-printer-2022
download drivers  + scripts
  
Add-PrinterPort -Name “IP_192.168.17.150” -PrinterHostAddress “192.168.17.150”
Add-PrinterPort -Name “IP_192.168.17.151” -PrinterHostAddress “192.168.17.151”
Add-PrinterPort -Name “IP_192.168.17.152” -PrinterHostAddress “192.168.17.152”
Add-Printer -Name Finance -DriverName “HP DJ 3700 series PCL-3” -PortName IP_192.168.17.150
Add-Printer -Name Marketing -DriverName “HP Color LaserJet Pro MFP M477 PCL 6” -PortName IP_192.168.17.151
Add-Printer -Name Operations -DriverName “Kyocera ECOSYS M3645idn XPS” -PortName IP_192.168.17.152



search for printer ports:
Get-PrinterPort

delete ports example:
Remove-PrinterPort -Name "HPBB2DE1"
Remove-PrinterPort -Name "1.1.1.1"

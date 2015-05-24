#Client Name

##Physical

They're located at 123 Main St. and will be for some time.

##Data Link

##Network

###Perimeter
They have 1 Cisco ASA. Here are the basics:

| Make | Model | Address |
|------|-------|---------|
|Cisco |ASA 5505| ```192.168.3.254```|


##Transport

##Applications

This is where we'll put application(s) info.

###Quickbooks

<div><p>Adding some crazy div!</p></div>

<strong>something strong</strong>

<h4 style="color:blue">This is a Blue Heading</h4>

##Desktop

###Login Scripts

```Powershell
# WMI query to list all properties and values of the Win32_BIOS class
# This PowerShell script was generated using the WMI Code Generator, Version 1.30
# http://www.robvanderwoude.com/updates/wmigen.html

param( [string]$strComputer = "." )

$colItems = get-wmiobject -class "Win32_BIOS" -namespace "root\CIMV2" -computername $strComputer

foreach ($objItem in $colItems) {
	write-host "Name                           :" $objItem.Name
	write-host "Version                        :" $objItem.Version
	write-host "Manufacturer                   :" $objItem.Manufacturer
	write-host "SMBIOSBIOS Version             :" $objItem.SMBIOSBIOSVersion
	write-host
}
```

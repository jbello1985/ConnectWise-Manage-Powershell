# New-CWMCompanyTeam
## SYNOPSIS
This function will create a new ticket.
## SYNTAX
```powershell
New-CWMCompanyTeam [-CompanyID] <Object> [[-id] <Int32>] [[-company] <Object>] [-teamRole] <Object> [[-locationId] <Int32>] [[-businessUnitId] <Int32>] [[-contact] <Object>] [[-member] <Object>] [[-accountManagerFlag] <Boolean>] [[-techFlag] <Boolean>] [[-salesFlag] <Boolean>] [[-_info] <Object>] [<CommonParameters>]
```
## PARAMETERS
### -CompanyID &lt;Object&gt;

```
Required                    true
Position                    1
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -id &lt;Int32&gt;

```
Required                    false
Position                    2
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -company &lt;Object&gt;

```
Required                    false
Position                    3
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -teamRole &lt;Object&gt;

```
Required                    true
Position                    4
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -locationId &lt;Int32&gt;

```
Required                    false
Position                    5
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -businessUnitId &lt;Int32&gt;

```
Required                    false
Position                    6
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -contact &lt;Object&gt;

```
Required                    false
Position                    7
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -member &lt;Object&gt;

```
Required                    false
Position                    8
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -accountManagerFlag &lt;Boolean&gt;

```
Required                    false
Position                    9
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -techFlag &lt;Boolean&gt;

```
Required                    false
Position                    10
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -salesFlag &lt;Boolean&gt;

```
Required                    false
Position                    11
Default value                False
Accept pipeline input       false
Accept wildcard characters  false
```
### -_info &lt;Object&gt;

```
Required                    false
Position                    12
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>$Ticket = @{

'identifier' = $Product.offerName
    'description' = $Product.offerName
    'subcategory' = @{id = 152}
    'type' = @{id = 47}
    'customerDescription' = $Product.offerName
    'cost' = $Product.unitPrice
    'price' = $Price
    'manufacturerPartNumber' = $Product.offerName
    'manufacturer' = $Manufacturer
    'productClass' = 'Agreement'
    'taxableFlag' = $true
}
New-CWTicket @Ticket
```

## NOTES
Author: Chris Taylor

Date: 8/22/2018 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/manage/rest?a=Company&e=CompanyTeams&o=CREATE

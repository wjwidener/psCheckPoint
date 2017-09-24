# New-CheckPointMulticastAddressRange

## SYNOPSIS
Create new object.

## SYNTAX

```
New-CheckPointMulticastAddressRange [-IPAddressFirst <String>] [-IPAddressLast <String>]
 [-IPv4AddressFirst <String>] [-IPv4AddressLast <String>] [-IPv6AddressFirst <String>]
 [-IPv6AddressLast <String>] [-Groups <String[]>] [-SetIfExists] -Name <String> [-Tags <String[]>]
 [-Comments <String>] [-IgnoreWarnings] [-IgnoreErrors] [-Color <String>] [-Session] <CheckPointSession>
```

## DESCRIPTION

## EXAMPLES

### ----------  EXAMPLE 1  ----------
```

```

## PARAMETERS

### -Color
Color of the object.
Should be one of existing colors.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Colour

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Comments
Comments string.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Groups
Collection of group identifiers.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -IgnoreErrors
Apply changes ignoring errors.
You won't be able to publish such a changes.
If ignore-warnings flag was omitted - warnings will also be ignored.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IgnoreWarnings
Apply changes ignoring warnings.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -IPAddressFirst
First IP address in the range.
If both IPv4 and IPv6 address ranges are required, use the ipv4-address-first and the ipv6-address-first fields instead.

```yaml
Type: String
Parameter Sets: (All)
Aliases: IPAddress

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -IPAddressLast
Last IP address in the range.
If both IPv4 and IPv6 address ranges are required, use the ipv4-address-first and the ipv6-address-first fields instead.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -IPv4AddressFirst
First IPv4 address in the range.

```yaml
Type: String
Parameter Sets: (All)
Aliases: IPv4Address

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -IPv4AddressLast
Last IPv4 address in the range.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -IPv6AddressFirst
First IPv6 address in the range.

```yaml
Type: String
Parameter Sets: (All)
Aliases: IPv6Address

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -IPv6AddressLast
Last IPv6 address in the range.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Object name.
Should be unique in the domain.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Session
Session object from Open-CheckPointSession

```yaml
Type: CheckPointSession
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SetIfExists
If another object with the same identifier already exists, it will be updated.
The command behaviour will be the same as if originally a set command was called.
Pay attention that original object's fields will be overwritten by the fields provided in the request payload!

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tags
Collection of tag identifiers.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

### System.String
First IP address in the range.
If both IPv4 and IPv6 address ranges are required, use the ipv4-address-first and the ipv6-address-first fields instead.

### System.String
Last IP address in the range.
If both IPv4 and IPv6 address ranges are required, use the ipv4-address-first and the ipv6-address-first fields instead.

### System.String
First IPv4 address in the range.

### System.String
Last IPv4 address in the range.

### System.String
First IPv6 address in the range.

### System.String
Last IPv6 address in the range.

### System.String[]
Collection of group identifiers.

### System.String
Object name.
Should be unique in the domain.

### System.String[]
Collection of tag identifiers.

### System.String
Comments string.

### System.String
Color of the object.
Should be one of existing colors.

## OUTPUTS

### psCheckPoint.Objects.MulticastAddressRange.CheckPointMulticastAddressRange
Details of a Check Point Multicast Address Range

## NOTES

## RELATED LINKS

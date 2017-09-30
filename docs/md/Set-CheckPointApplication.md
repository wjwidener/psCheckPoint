# Set-CheckPointApplication

## SYNOPSIS
Edit existing object using object name or uid.

## SYNTAX

### Base Details Only (Default)
```
Set-CheckPointApplication [-GroupAction <MembershipActions>] [-Groups <String[]>] [-PrimaryCategory <String>]
 [-UrlAction <MembershipActions>] [-ApplicationSignatureAction <MembershipActions>]
 [-AdditionalCategoriesAction <MembershipActions>] [-AdditionalCategories <String[]>] [-Description <String>]
 [-UrlsDefinedAsRegularExpression] [-NewName <String>] [-Tags <String[]>] [-Comments <String>]
 [-IgnoreWarnings] [-IgnoreErrors] [-Color <String>] [-Session] <CheckPointSession>
```

### By URLs
```
Set-CheckPointApplication [-GroupAction <MembershipActions>] [-Groups <String[]>] [-PrimaryCategory <String>]
 [-UrlAction <MembershipActions>] [-UrlList <String[]>] [-ApplicationSignatureAction <MembershipActions>]
 [-AdditionalCategoriesAction <MembershipActions>] [-AdditionalCategories <String[]>] [-Description <String>]
 [-UrlsDefinedAsRegularExpression] [-NewName <String>] [-Tags <String[]>] [-Comments <String>]
 [-IgnoreWarnings] [-IgnoreErrors] [-Color <String>] [-Session] <CheckPointSession>
```

### By Application Signature
```
Set-CheckPointApplication [-GroupAction <MembershipActions>] [-Groups <String[]>] [-PrimaryCategory <String>]
 [-UrlAction <MembershipActions>] [-ApplicationSignatureAction <MembershipActions>]
 [-ApplicationSignature <String[]>] [-AdditionalCategoriesAction <MembershipActions>]
 [-AdditionalCategories <String[]>] [-Description <String>] [-UrlsDefinedAsRegularExpression]
 [-NewName <String>] [-Tags <String[]>] [-Comments <String>] [-IgnoreWarnings] [-IgnoreErrors]
 [-Color <String>] [-Session] <CheckPointSession>
```

### By UID
```
Set-CheckPointApplication [-GroupAction <MembershipActions>] [-Groups <String[]>] [-PrimaryCategory <String>]
 [-UrlAction <MembershipActions>] [-ApplicationSignatureAction <MembershipActions>]
 [-AdditionalCategoriesAction <MembershipActions>] [-AdditionalCategories <String[]>] [-Description <String>]
 [-UrlsDefinedAsRegularExpression] -UID <String> [-NewName <String>] [-Tags <String[]>] [-Comments <String>]
 [-IgnoreWarnings] [-IgnoreErrors] [-Color <String>] [-Session] <CheckPointSession>
```

### By Name
```
Set-CheckPointApplication [-GroupAction <MembershipActions>] [-Groups <String[]>] [-PrimaryCategory <String>]
 [-UrlAction <MembershipActions>] [-ApplicationSignatureAction <MembershipActions>]
 [-AdditionalCategoriesAction <MembershipActions>] [-AdditionalCategories <String[]>] [-Description <String>]
 [-UrlsDefinedAsRegularExpression] [-Name] <String> [-NewName <String>] [-Tags <String[]>] [-Comments <String>]
 [-IgnoreWarnings] [-IgnoreErrors] [-Color <String>] [-Session] <CheckPointSession>
```

## DESCRIPTION

## EXAMPLES

### ----------  EXAMPLE 1  ----------
```

```

## PARAMETERS

### -AdditionalCategories
Used to configure or edit the additional categories of a custom application / site used in the Application and URL Filtering or Threat Prevention.

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

### -AdditionalCategoriesAction
Action to take with Additional Categories.

Possible values: Replace, Add, Remove

```yaml
Type: MembershipActions
Parameter Sets: (All)
Aliases: 
Accepted values: Replace, Add, Remove

Required: False
Position: Named
Default value: Replace
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationSignature
Application signature generated by Signature Tool.

```yaml
Type: String[]
Parameter Sets: By Application Signature
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApplicationSignatureAction
Action to take with Application Signatures.

Possible values: Replace, Add, Remove

```yaml
Type: MembershipActions
Parameter Sets: (All)
Aliases: 
Accepted values: Replace, Add, Remove

Required: False
Position: Named
Default value: Replace
Accept pipeline input: False
Accept wildcard characters: False
```

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

### -Description
A description for the application.

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

### -GroupAction
Action to take with groups.

Possible values: Replace, Add, Remove

```yaml
Type: MembershipActions
Parameter Sets: (All)
Aliases: 
Accepted values: Replace, Add, Remove

Required: False
Position: Named
Default value: Replace
Accept pipeline input: False
Accept wildcard characters: False
```

### -Groups
Collection of group identifiers.

Groups listed will be either Added, Removed or replace the current list of group membership based on GroupAction parameter.

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

### -Name
Object name.

```yaml
Type: String
Parameter Sets: By Name
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -NewName
New name of the object.

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

### -PrimaryCategory
Each application is assigned to one primary category based on its most defining aspect.

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

### -UID
Object unique identifier.

```yaml
Type: String
Parameter Sets: By UID
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UrlAction
Action to take with URLs.

Possible values: Replace, Add, Remove

```yaml
Type: MembershipActions
Parameter Sets: (All)
Aliases: 
Accepted values: Replace, Add, Remove

Required: False
Position: Named
Default value: Replace
Accept pipeline input: False
Accept wildcard characters: False
```

### -UrlList
URLs that determine this particular application.

```yaml
Type: String[]
Parameter Sets: By URLs
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UrlsDefinedAsRegularExpression
States whether the URL is defined as a Regular Expression or not.

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

## INPUTS

### System.String[]
Collection of group identifiers.

Groups listed will be either Added, Removed or replace the current list of group membership based on GroupAction parameter.

### System.String
Each application is assigned to one primary category based on its most defining aspect.

### System.String[]
URLs that determine this particular application.

### System.String[]
Application signature generated by Signature Tool.

### System.String[]
Used to configure or edit the additional categories of a custom application / site used in the Application and URL Filtering or Threat Prevention.

### System.String
A description for the application.

### System.String
Object unique identifier.

### System.String
Object name.

### System.String
New name of the object.

### System.String[]
Collection of tag identifiers.

### System.String
Comments string.

### System.String
Color of the object.
Should be one of existing colors.

## OUTPUTS

### psCheckPoint.Objects.Application.CheckPointApplication
Details of a Check Point Application/Site

## NOTES

## RELATED LINKS

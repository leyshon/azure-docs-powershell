---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
online version: 
schema: 2.0.0
---

# Get-AzureRmProviderFeature

## SYNOPSIS
{{Fill in the Synopsis}}

## SYNTAX

### ListAvailableParameterSet (Default)
```
Get-AzureRmProviderFeature [-ProviderNamespace <String>] [-ListAvailable] [<CommonParameters>]
```

### GetFeature
```
Get-AzureRmProviderFeature -ProviderNamespace <String> -FeatureName <String> [<CommonParameters>]
```

## DESCRIPTION
{{Fill in the Description}}

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -FeatureName
The feature name.

```yaml
Type: String
Parameter Sets: GetFeature
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ListAvailable
When set, lists all available features including those not registered with the current subscription.

```yaml
Type: SwitchParameter
Parameter Sets: ListAvailableParameterSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProviderNamespace
The resource provider namespace.

```yaml
Type: String
Parameter Sets: ListAvailableParameterSet
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: GetFeature
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### System.Collections.Generic.List`1[[Microsoft.Azure.Commands.Resources.Models.ProviderFeatures.PSProviderFeature, Microsoft.Azure.Commands.Resources, Version=1.0.4.3, Culture=neutral, PublicKeyToken=31bf3856ad364e35]]

## NOTES

## RELATED LINKS


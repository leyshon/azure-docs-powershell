---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 700AA986-6C66-4BB1-8605-605875CD53C4
---

# Remove-AzureDeployment

## SYNOPSIS
Deletes a deployment of a cloud service.

## SYNTAX

```
Remove-AzureDeployment [-ServiceName] <String> [-Slot] <String> [-DeleteVHD] [-Force]
 [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureDeployment** cmdlet deletes a deployment of an Azure cloud service.
To delete a deployment, first suspend it.

## EXAMPLES

### Example 1: Remove a deployment
```
PS C:\>Remove-AzureDeployment -ServiceName "ContosoService"
```

This command removes the deployment of the Azure service named ContosoService.
Because this command does not specify a slot, it removes the service from the production environment.

### Example 2: Remove a deployment and virtual hard disks
```
PS C:\>Remove-AzureDeployment -ServiceName "ContosoService" -DeleteVHD
```

This command removes the deployment of the service named ContosoService from the production environment.
The command also removes the underlying virtual hard disks.

## PARAMETERS

### -ServiceName
Specifies the name of the service for which this cmdlet deletes a deployment.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Specifies the deployment environment from which this cmdlet deletes the deployment.
Valid values are: Staging and Production.
The default value is Production.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DeleteVHD
Specifies that this cmdlet removes the deployment and the virtual hard disks (VHDs) from blob storage.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
ps_force

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
ps_azureprofile_description

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### ManagementOperationContext

## NOTES

## RELATED LINKS

[Get-AzureDeployment](./Get-AzureDeployment.md)

[Get-AzureDeploymentEvent](./Get-AzureDeploymentEvent.md)

[Move-AzureDeployment](./Move-AzureDeployment.md)

[New-AzureDeployment](./New-AzureDeployment.md)

[Set-AzureDeployment](./Set-AzureDeployment.md)



---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
Module Name: AzureRM.SiteRecovery
ms.assetid: 77F1556C-323D-49CA-BD6C-75B2D4E0F894
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/SiteRecovery/Commands.SiteRecovery/help/Get-AzureRmSiteRecoveryProtectionContainer.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/SiteRecovery/Commands.SiteRecovery/help/Get-AzureRmSiteRecoveryProtectionContainer.md
---

# Get-AzureRmSiteRecoveryProtectionContainer

## SYNOPSIS
Gets protection containers for the current Site Recovery vault.

## SYNTAX

### Default (Default)
```
Get-AzureRmSiteRecoveryProtectionContainer [-DefaultProfile <IAzureContextContainer>] [<CommonParameters>]
```

### ByObjectWithName
```
Get-AzureRmSiteRecoveryProtectionContainer -Name <String> -Fabric <ASRFabric>
 [-DefaultProfile <IAzureContextContainer>] [<CommonParameters>]
```

### ByObjectWithNameLegacy
```
Get-AzureRmSiteRecoveryProtectionContainer -Name <String> [-DefaultProfile <IAzureContextContainer>]
 [<CommonParameters>]
```

### ByObjectWithFriendlyName
```
Get-AzureRmSiteRecoveryProtectionContainer -FriendlyName <String> -Fabric <ASRFabric>
 [-DefaultProfile <IAzureContextContainer>] [<CommonParameters>]
```

### ByObjectWithFriendlyNameLegacy
```
Get-AzureRmSiteRecoveryProtectionContainer -FriendlyName <String> [-DefaultProfile <IAzureContextContainer>]
 [<CommonParameters>]
```

### ByFabricObject
```
Get-AzureRmSiteRecoveryProtectionContainer -Fabric <ASRFabric> [-DefaultProfile <IAzureContextContainer>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmSiteRecoveryProtectionContainer** cmdlet gets protection containers for the current Azure Site Recovery vault.
A protection container is a logical container for protected objects such as virtual machines.
Protection policies define replication settings for protected items and can be associated with a protection container and applied to a protected entity.

## EXAMPLES

## PARAMETERS

### -Fabric
```yaml
Type: Microsoft.Azure.Commands.SiteRecovery.ASRFabric
Parameter Sets: ByObjectWithName, ByObjectWithFriendlyName, ByFabricObject
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -FriendlyName
Specifies the friendly name of the protection container.

```yaml
Type: System.String
Parameter Sets: ByObjectWithFriendlyName, ByObjectWithFriendlyNameLegacy
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the protection container.

```yaml
Type: System.String
Parameter Sets: ByObjectWithName, ByObjectWithNameLegacy
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with azure.

```yaml
Type: Microsoft.Azure.Commands.Common.Authentication.Abstractions.IAzureContextContainer
Parameter Sets: (All)
Aliases: AzureRmContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### ASRFabric
Parameter 'Fabric' accepts value of type 'ASRFabric' from the pipeline

## OUTPUTS

### System.Collections.Generic.IEnumerable`1[Microsoft.Azure.Commands.SiteRecovery.ASRProtectionContainer]

## NOTES

## RELATED LINKS


---
external help file: Microsoft.Azure.Commands.ResourceManager.Automation.dll-Help.xml
Module Name: AzureRM.Automation
ms.assetid: 739EB137-E4A8-4E85-96BD-4CF26D2C5763
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Automation/Commands.Automation/help/New-AzureRMAutomationCredential.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Automation/Commands.Automation/help/New-AzureRMAutomationCredential.md
---

# New-AzureRmAutomationCredential

## SYNOPSIS
Creates an Automation credential.

## SYNTAX

```
New-AzureRmAutomationCredential [-Name] <String> [-Description <String>] [-Value] <PSCredential>
 [-ResourceGroupName] <String> [-AutomationAccountName] <String> [-DefaultProfile <IAzureContextContainer>]
 [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmAutomationCredential** cmdlet creates a credential as a **PSCredential** object in Azure Automation.

## EXAMPLES

### Example 1: Create a credential
```
PS C:\>$User = "Contoso\PFuller"
PS C:\> $Password = ConvertTo-SecureString "Password" -AsPlainText -Force
PS C:\> $Credential = New-Object -TypeName System.Management.Automation.PSCredential -ArgumentList $User, $Password
PS C:\> New-AzureRmAutomationCredential -AutomationAccountName "Contoso17" -Name "ContosoCredential" -Value $Credential -ResourceGroupName "ResourceGroup01"
```

The first command assigns a user name to the $User variable.

The second command converts a plain text password into a secure string by using the ConvertTo-SecureString cmdlet.
The command stores that object in the $Password variable.

The third command creates a credential based on $User and $Password, and then stores it in the $Credential variable.

The final command creates an Automation credential named ContosoCredential that uses $Credential.

## PARAMETERS

### -AutomationAccountName
Specifies the name of the Automation account in which this cmdlet stores the credential.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Description
Specifies a description for the credential.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies a name for the credential.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies a description for the resource group for which this cmdlet creates a credential.

```yaml
Type: System.String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Value
Specifies the credentials as a **PSCredential** object.

```yaml
Type: System.Management.Automation.PSCredential
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
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

## OUTPUTS

### Microsoft.Azure.Commands.Automation.Model.CredentialInfo

## NOTES

## RELATED LINKS

[Get-AzureRmAutomationCredential](./Get-AzureRMAutomationCredential.md)

[Remove-AzureRmAutomationCredential](./Remove-AzureRMAutomationCredential.md)

[Set-AzureRmAutomationCredential](./Set-AzureRMAutomationCredential.md)



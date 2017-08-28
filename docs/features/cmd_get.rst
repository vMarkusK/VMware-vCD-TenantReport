Get Commands
=========================

This page contains details on **Get** commands.

Get-VcdTenantReport
-------------------------


NAME
    Get-VcdTenantReport
    
SYNOPSIS
    
    
SYNTAX
    Get-VcdTenantReport [-Server] <String> [-Org] <String> [[-Credential] <PSCredential>] [[-Path] <String>] [<CommonParameters>]
    
    
DESCRIPTION
    This Function creates a HTML Report for your vCloud Director Organization.
    
    This Function is fully tested as Organization Administrator.
    With lower permissions a unexpected behavior is possible.
    

PARAMETERS
    -Server <String>
        The FQDN of your vCloud Director Endpoint.
        
    -Org <String>
        The Organization Name.
        
    -Credential <PSCredential>
        PowerShell Credentials to access the EÃ©nvironment.
        
    -Path <String>
        The Path of the exported HTML Report.
        
        
        Requires -Version 5
        Requires -Modules VMware.VimAutomation.Cloud, @{ModuleName="VMware.VimAutomation.Cloud";ModuleVersion="6.5.1.0"}
        
    <CommonParameters>
        This cmdlet supports the common parameters: Verbose, Debug,
        ErrorAction, ErrorVariable, WarningAction, WarningVariable,
        OutBuffer, PipelineVariable, and OutVariable. For more information, see 
        about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216). 
    
    -------------------------- EXAMPLE 1 --------------------------
    
    PS C:\>Get-VcdTenantReport -Server $ServerFQDN -Org $OrgName -Credential $MyCedential
    
    
    
    
    
    
    -------------------------- EXAMPLE 2 --------------------------
    
    PS C:\>Get-VcdTenantReport -Server $ServerFQDN -Org $OrgName -Path "C:\Temp\Report.html"
    
    
    
    
    
    
REMARKS
    To see the examples, type: "get-help Get-VcdTenantReport -examples".
    For more information, type: "get-help Get-VcdTenantReport -detailed".
    For technical information, type: "get-help Get-VcdTenantReport -full".





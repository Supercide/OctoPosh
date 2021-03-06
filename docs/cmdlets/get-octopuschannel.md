﻿
### Summary

Gets information about Octopus Channels
### Parameters
| Name | DataType          | Description |
| ------------- | ----------- | ----------- |
| ChannelName | String[] |  Channel name     |
| ProjectName | String[] |  Project name     |
| ResourceOnly | Switch |  If set to TRUE the cmdlet will return the basic Octopur resource. If not set or set to FALSE, the  cmdlet will return a human friendly Octoposh output object     |

### Syntax
``` powershell

Get-OctopusChannel [[-ChannelName] <string[]>] [[-ProjectName] <string[]>] [-ResourceOnly 
<SwitchParameter>] [<CommonParameters>]




``` 

### Examples 

**EXAMPLE 1**

Gets all the channels in all the projects of the instance

``` powershell 
 Get-OctopusChannel
``` 

**EXAMPLE 2**

Gets all the channels of the project "MyFinantialApp"

``` powershell 
 Get-OctopusChannel -Project "MyFinantialApp"
``` 

**EXAMPLE 3**

Gets the Channel with the name "Hotfix_Website" of the project "MyFinantialApp"

``` powershell 
 Get-OctopusChannel -name "Hotfix_Website" -Project "MyFinantialApp"
``` 

**EXAMPLE 4**

Gets the Channels with the names "Hotfix_Website" and "Hotfix_WebService" of the project "MyFinantialApp"

``` powershell 
 Get-OctopusChannel -name "Hotfix_Website","Hotfix_WebService" -Project "MyFinantialApp"
``` 

**EXAMPLE 5**

Gets all the Channels whose name starts with "Hotfix_" of the project "MyFinantialApp"

``` powershell 
 Get-OctopusChannel -name "Hotfix_*" -Project "MyFinantialApp"
``` 


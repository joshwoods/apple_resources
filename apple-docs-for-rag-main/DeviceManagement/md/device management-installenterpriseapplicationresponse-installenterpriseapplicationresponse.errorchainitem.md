

- Device Management
- InstallEnterpriseApplicationResponse
-  InstallEnterpriseApplicationResponse.ErrorChainItem 

Device Management Command

# InstallEnterpriseApplicationResponse.ErrorChainItem

A dictionary that describes an error chain item.

macOS 10.13.6+Device Assignment ServicesVPP License Management

``` source
object InstallEnterpriseApplicationResponse.ErrorChainItem
```

## Properties

`ErrorCode`

`integer`

 (Required) 

The error code.

`ErrorDomain`

`string`

 (Required) 

The error domain.

`LocalizedDescription`

`string`

 (Required) 

A description of the error in the device’s localized language.

`USEnglishDescription`

`string`

A description of the error in U.S. English.


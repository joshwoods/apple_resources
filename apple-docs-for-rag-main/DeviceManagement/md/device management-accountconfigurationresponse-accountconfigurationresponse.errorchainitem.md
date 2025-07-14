

- Device Management
- AccountConfigurationResponse
-  AccountConfigurationResponse.ErrorChainItem 

Device Management Command

# AccountConfigurationResponse.ErrorChainItem

A dictionary that describes an error chain item.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object AccountConfigurationResponse.ErrorChainItem
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


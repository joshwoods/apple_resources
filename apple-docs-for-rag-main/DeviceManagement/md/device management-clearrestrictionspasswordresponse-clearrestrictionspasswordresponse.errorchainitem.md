

- Device Management
- ClearRestrictionsPasswordResponse
-  ClearRestrictionsPasswordResponse.ErrorChainItem 

Device Management Command

# ClearRestrictionsPasswordResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 8.0+iPadOS 8.0+Device Assignment ServicesVPP License Management

``` source
object ClearRestrictionsPasswordResponse.ErrorChainItem
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




- Device Management
- DisableRemoteDesktopResponse
-  DisableRemoteDesktopResponse.ErrorChainItem 

Device Management Command

# DisableRemoteDesktopResponse.ErrorChainItem

A dictionary that describes an error chain item.

macOS 10.14.4+Device Assignment ServicesVPP License Management

``` source
object DisableRemoteDesktopResponse.ErrorChainItem
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


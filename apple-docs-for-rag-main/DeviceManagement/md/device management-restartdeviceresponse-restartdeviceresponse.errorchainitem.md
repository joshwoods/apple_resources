

- Device Management
- RestartDeviceResponse
-  RestartDeviceResponse.ErrorChainItem 

Device Management Command

# RestartDeviceResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 10.3+iPadOS 10.3+macOS 10.13+tvOS 10.2+Device Assignment ServicesVPP License Management

``` source
object RestartDeviceResponse.ErrorChainItem
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


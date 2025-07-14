

- Device Management
- DeviceLockResponse
-  DeviceLockResponse.ErrorChainItem 

Device Management Command

# DeviceLockResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 4.0+iPadOS 4.0+macOS 10.7+visionOS 2.0+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeviceLockResponse.ErrorChainItem
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


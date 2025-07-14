

- Device Management
- DeviceConfiguredResponse
-  DeviceConfiguredResponse.ErrorChainItem 

Device Management Command

# DeviceConfiguredResponse.ErrorChainItem

A dictionary that describes an error chain.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 10.2+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object DeviceConfiguredResponse.ErrorChainItem
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


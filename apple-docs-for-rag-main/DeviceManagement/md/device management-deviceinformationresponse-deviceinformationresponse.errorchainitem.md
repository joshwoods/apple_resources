

- Device Management
- DeviceInformationResponse
-  DeviceInformationResponse.ErrorChainItem 

Device Management Command

# DeviceInformationResponse.ErrorChainItem

A dictionary that describes an error chain.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeviceInformationResponse.ErrorChainItem
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

## See Also

### Commands

object DeviceInformationResponse.QueryResponses

The response dictionary that contains information about the device.


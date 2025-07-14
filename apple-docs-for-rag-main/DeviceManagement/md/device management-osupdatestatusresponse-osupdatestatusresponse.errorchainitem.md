

- Device Management
- OSUpdateStatusResponse
-  OSUpdateStatusResponse.ErrorChainItem 

Device Management Command

# OSUpdateStatusResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 9.0+iPadOS 9.0+macOS 10.11.5+tvOS 12.0+Device Assignment ServicesVPP License Management

``` source
object OSUpdateStatusResponse.ErrorChainItem
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

object OSUpdateStatusResponse.OSUpdateStatusItem

A dictionary that describes the status of a software update.


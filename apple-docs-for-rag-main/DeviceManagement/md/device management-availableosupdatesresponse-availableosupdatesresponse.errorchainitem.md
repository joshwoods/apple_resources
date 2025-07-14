

- Device Management
- AvailableOSUpdatesResponse
-  AvailableOSUpdatesResponse.ErrorChainItem 

Device Management Command

# AvailableOSUpdatesResponse.ErrorChainItem

A dictionary that describes an error chain item.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 12.0+Device Assignment ServicesVPP License Management

``` source
object AvailableOSUpdatesResponse.ErrorChainItem
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

object AvailableOSUpdatesResponse.AvailableOSUpdatesItem

The response dictionary that describes the available operating-system updates item.


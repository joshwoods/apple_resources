

- Device Management
- LOMDeviceRequestResponse
-  LOMDeviceRequestResponse.ErrorChainItem 

Device Management Command

# LOMDeviceRequestResponse.ErrorChainItem

A dictionary that describes an error chain item.

macOS 11.0+Device Assignment ServicesVPP License Management

``` source
object LOMDeviceRequestResponse.ErrorChainItem
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

object LOMDeviceRequestResponse.ResponseListItem

A dictionary that describes a response list item.


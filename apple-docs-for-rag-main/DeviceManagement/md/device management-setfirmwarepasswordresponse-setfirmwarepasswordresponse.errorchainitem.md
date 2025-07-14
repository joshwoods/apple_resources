

- Device Management
- SetFirmwarePasswordResponse
-  SetFirmwarePasswordResponse.ErrorChainItem 

Device Management Command

# SetFirmwarePasswordResponse.ErrorChainItem

A dictionary that describes an error chain item.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object SetFirmwarePasswordResponse.ErrorChainItem
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

object SetFirmwarePasswordResponse.SetFirmwarePassword

A dictionary that describes the result of a command to change the firmware password.


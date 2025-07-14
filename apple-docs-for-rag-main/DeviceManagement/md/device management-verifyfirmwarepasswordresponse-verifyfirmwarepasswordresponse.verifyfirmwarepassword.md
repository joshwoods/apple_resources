

- Device Management
- VerifyFirmwarePasswordResponse
-  VerifyFirmwarePasswordResponse.VerifyFirmwarePassword 

Device Management Command

# VerifyFirmwarePasswordResponse.VerifyFirmwarePassword

A dictionary that describes the result of a command to verify the firmware password.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object VerifyFirmwarePasswordResponse.VerifyFirmwarePassword
```

## Properties

`PasswordVerified`

`boolean`

 (Required) 

If `true`, the provided password matched the firmware password set for the device.

## See Also

### Commands

object VerifyFirmwarePasswordResponse.ErrorChainItem

A dictionary that describes an error chain item.


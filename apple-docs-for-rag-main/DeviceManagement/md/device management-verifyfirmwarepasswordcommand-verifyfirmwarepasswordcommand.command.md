

- Device Management
- VerifyFirmwarePasswordCommand
-  VerifyFirmwarePasswordCommand.Command 

Device Management Command

# VerifyFirmwarePasswordCommand.Command

The request dictionary to verify the firmware password.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object VerifyFirmwarePasswordCommand.Command
```

## Properties

`Password`

`string`

 (Required) 

The password to verify.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to verify the firmware password.

Value: `VerifyFirmwarePassword`




- Device Management
- SetFirmwarePasswordCommand
-  SetFirmwarePasswordCommand.Command 

Device Management Command

# SetFirmwarePasswordCommand.Command

The request dictionary to change or clear the firmware password.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object SetFirmwarePasswordCommand.Command
```

## Properties

`AllowOroms`

`boolean`

If `true`, enable ROMs.

Default: `false`

`CurrentPassword`

`string`

The current password, which you must set if the device has a firmware password.

`NewPassword`

`string`

 (Required) 

The new firmware password. Set to an empty string to clear the password. The characters in this value must consist of low-ASCII, printable characters (`0x20` through `0x7E`) to ensure that all characters are enterable on the EFI login screen.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to change or clear the firmware password.

Value: `SetFirmwarePassword`


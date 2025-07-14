

- Device Management
- EnableRemoteDesktopCommand
-  EnableRemoteDesktopCommand.Command 

Device Management Command

# EnableRemoteDesktopCommand.Command

The request dictionary to enable Remote Desktop on a device.

macOS 10.14.4+Device Assignment ServicesVPP License Management

``` source
object EnableRemoteDesktopCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to enable Remote Desktop on a device.

Value: `EnableRemoteDesktop`




- Device Management
- DisableRemoteDesktopCommand
-  DisableRemoteDesktopCommand.Command 

Device Management Command

# DisableRemoteDesktopCommand.Command

The request dictionary to disable Remote Desktop on a device.

macOS 10.14.4+Device Assignment ServicesVPP License Management

``` source
object DisableRemoteDesktopCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to disable Remote Desktop on a device.

Value: `DisableRemoteDesktop`


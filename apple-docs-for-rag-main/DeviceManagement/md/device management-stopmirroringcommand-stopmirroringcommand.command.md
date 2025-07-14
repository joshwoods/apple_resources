

- Device Management
- StopMirroringCommand
-  StopMirroringCommand.Command 

Device Management Command

# StopMirroringCommand.Command

The request dictionary to stop mirroring the display on another device.

iOS 7.0+iPadOS 7.0+macOS 10.10+Device Assignment ServicesVPP License Management

``` source
object StopMirroringCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to stop mirroring the display on another device.

Value: `StopMirroring`


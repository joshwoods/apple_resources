

- Device Management
- RequestMirroringCommand
-  RequestMirroringCommand.Command 

Device Management Command

# RequestMirroringCommand.Command

The request dictionary to prompt the user to share their screen using AirPlay Mirroring.

iOS 7.0+iPadOS 7.0+macOS 10.10+Device Assignment ServicesVPP License Management

``` source
object RequestMirroringCommand.Command
```

## Properties

`DestinationName`

`string`

The name of the AirPlay Mirroring destination.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to prompt the user to share their screen using AirPlay Mirroring.

Value: `RequestMirroring`

`DestinationDeviceID`

`string`

The hardware address of the AirPlay Mirroring destination that identifies the device, in the format `xx:xx:xx:xx:xx`. This value isn’t case-sensitive.

`Password`

`string`

The screen-sharing password that the device uses when connecting to the destination.

`ScanTime`

`integer`

The number of seconds, from `10` to `300`, for the device to spend searching for the destination. The default value is `30`.


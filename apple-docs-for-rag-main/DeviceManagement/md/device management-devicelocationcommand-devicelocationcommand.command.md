

- Device Management
- DeviceLocationCommand
-  DeviceLocationCommand.Command 

Device Management Command

# DeviceLocationCommand.Command

The request dictionary to request a device’s location.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

``` source
object DeviceLocationCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to request a device’s location.

Value: `DeviceLocation`




- Device Management
- ShutDownDeviceCommand
-  ShutDownDeviceCommand.Command 

Device Management Command

# ShutDownDeviceCommand.Command

The request dictionary to shut down a device.

iOS 10.3+iPadOS 10.3+macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object ShutDownDeviceCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to shut down a device.

Value: `ShutDownDevice`


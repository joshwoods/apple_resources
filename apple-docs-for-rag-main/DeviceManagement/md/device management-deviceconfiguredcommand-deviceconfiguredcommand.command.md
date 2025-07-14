

- Device Management
- DeviceConfiguredCommand
-  DeviceConfiguredCommand.Command 

Device Management Command

# DeviceConfiguredCommand.Command

The request dictionary to inform a device that it can allow the user to continue in Setup Assistant.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 10.2+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object DeviceConfiguredCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to inform a device that it can allow the user to continue in Setup Assistant.

Value: `DeviceConfigured`


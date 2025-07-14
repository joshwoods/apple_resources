

- Device Management
- SecurityInfoCommand
-  SecurityInfoCommand.Command 

Device Management Command

# SecurityInfoCommand.Command

The request dictionary to get security-related information about a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SecurityInfoCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get security-related information about a device.

Value: `SecurityInfo`


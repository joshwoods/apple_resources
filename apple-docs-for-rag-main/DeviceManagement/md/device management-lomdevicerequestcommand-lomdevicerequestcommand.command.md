

- Device Management
- LOMDeviceRequestCommand
-  LOMDeviceRequestCommand.Command 

Device Management Command

# LOMDeviceRequestCommand.Command

The request dictionary to send requests to a device using lights-out management (LOM).

macOS 11.0+Device Assignment ServicesVPP License Management

``` source
object LOMDeviceRequestCommand.Command
```

## Properties

`RequestList`

`[`LOMDeviceRequestCommand.Command.RequestListItem`]`

 (Required) 

An array of requests to perform.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to send requests to a device using lights-out management (LOM).

Value: `LOMDeviceRequest`

## Topics

### Commands

object LOMDeviceRequestCommand.Command.RequestListItem

A dictionary that contains a requested action to perform on a device using lights-out management (LOM).


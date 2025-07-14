

- Device Management
- LOMSetupRequestCommand
-  LOMSetupRequestCommand.Command 

Device Management Command

# LOMSetupRequestCommand.Command

The request dictionary to get information from a device to set up lights-out management (LOM).

macOS 11.0+Device Assignment ServicesVPP License Management

``` source
object LOMSetupRequestCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get information from a device to set up lights-out management (LOM).

Value: `LOMSetupRequest`


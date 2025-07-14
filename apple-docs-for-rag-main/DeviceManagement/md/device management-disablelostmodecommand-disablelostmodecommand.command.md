

- Device Management
- DisableLostModeCommand
-  DisableLostModeCommand.Command 

Device Management Command

# DisableLostModeCommand.Command

The request dictionary to disable Lost Mode.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

``` source
object DisableLostModeCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to disable Lost Mode.

Value: `DisableLostMode`


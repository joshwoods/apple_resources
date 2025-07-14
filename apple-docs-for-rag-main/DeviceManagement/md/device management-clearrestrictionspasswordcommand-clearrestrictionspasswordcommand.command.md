

- Device Management
- ClearRestrictionsPasswordCommand
-  ClearRestrictionsPasswordCommand.Command 

Device Management Command

# ClearRestrictionsPasswordCommand.Command

The request dictionary to clear a restrictions passcode.

iOS 8.0+iPadOS 8.0+Device Assignment ServicesVPP License Management

``` source
object ClearRestrictionsPasswordCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to clear a restrictions passcode.

Value: `ClearRestrictionsPassword`




- Device Management
- ClearPasscodeCommand
-  ClearPasscodeCommand.Command 

Device Management Command

# ClearPasscodeCommand.Command

The request dictionary to clear a passcode.

iOS 4.0+iPadOS 4.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ClearPasscodeCommand.Command
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

Value: `ClearPasscode`

`UnlockToken`

`data`

 (Required) 

The unlock token value that the device provides in its `TokenUpdateMessage` check-in message.




- Device Management
- PlayLostModeSoundCommand
-  PlayLostModeSoundCommand.Command 

Device Management Command

# PlayLostModeSoundCommand.Command

The request dictionary to play the Lost Mode sound.

iOS 10.3+iPadOS 10.3+Device Assignment ServicesVPP License Management

``` source
object PlayLostModeSoundCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to play the Lost Mode sound.

Value: `PlayLostModeSound`


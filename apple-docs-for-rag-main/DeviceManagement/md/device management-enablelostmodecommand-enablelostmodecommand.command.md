

- Device Management
- EnableLostModeCommand
-  EnableLostModeCommand.Command 

Device Management Command

# EnableLostModeCommand.Command

The request dictionary to enable Lost Mode.

iOS 9.3+iPadOS 9.3+Device Assignment ServicesVPP License Management

``` source
object EnableLostModeCommand.Command
```

## Properties

`Footnote`

`string`

If present, display this text in place of *Slide to Unlock*.

`Message`

`string`

If present, display this text on the Lock screen. You must provide this value if you don’t provide a value for `PhoneNumber`.

`PhoneNumber`

`string`

If present, display this phone number on the Lock screen. You must provide this value if you don’t provide a value for `Message`.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to enable Lost Mode.

Value: `EnableLostMode`




- Device Management
- ActiveNSExtensionsCommand
-  ActiveNSExtensionsCommand.Command 

Device Management Command

# ActiveNSExtensionsCommand.Command

The request dictionary to get a list of active extensions for a user on a device.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object ActiveNSExtensionsCommand.Command
```

## Properties

`FilterExtensionPoints`

`[string]`

An array of extension points. If you choose to provide this value, the response only includes the app extensions for the extension points you specify.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get a list of active app extensions for a user.

Value: `ActiveNSExtensions`


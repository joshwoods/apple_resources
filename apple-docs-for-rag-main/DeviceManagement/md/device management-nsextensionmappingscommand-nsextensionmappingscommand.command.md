

- Device Management
- NSExtensionMappingsCommand
-  NSExtensionMappingsCommand.Command 

Device Management Command

# NSExtensionMappingsCommand.Command

The request dictionary to get a list of the installed extensions for a user on a device.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object NSExtensionMappingsCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get a list of the installed extensions for a user.

Value: `NSExtensionMappings`


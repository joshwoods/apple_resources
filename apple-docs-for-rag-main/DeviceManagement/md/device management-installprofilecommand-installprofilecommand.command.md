

- Device Management
- InstallProfileCommand
-  InstallProfileCommand.Command 

Device Management Command

# InstallProfileCommand.Command

The request dictionary to install a configuration profile.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstallProfileCommand.Command
```

## Properties

`Payload`

`data`

 (Required) 

The profile to install, which you can encrypt using any identity certificate installed on the device. You can also sign the profile.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to install a profile.

Value: `InstallProfile`


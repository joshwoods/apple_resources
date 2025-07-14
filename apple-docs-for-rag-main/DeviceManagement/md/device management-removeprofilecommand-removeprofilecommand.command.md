

- Device Management
- RemoveProfileCommand
-  RemoveProfileCommand.Command 

Device Management Command

# RemoveProfileCommand.Command

The request dictionary to remove a profile.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object RemoveProfileCommand.Command
```

## Properties

`Identifier`

`string`

 (Required) 

The identifier of the profile to remove.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to remove a profile.

Value: `RemoveProfile`


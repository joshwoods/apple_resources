

- Device Management
- ProfileListCommand
-  ProfileListCommand.Command 

Device Management Command

# ProfileListCommand.Command

The request dictionary to get a list of installed profiles.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ProfileListCommand.Command
```

## Properties

`ManagedOnly`

`boolean`

If `true`, only include profiles that MDM has installed. For user enrollments, the device ignores this key and always limits the results to managed profiles. This value is available in iOS 13 and later, macOS 10.5 and later, and tvOS 13 and later.

Default: `false`

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get a list of installed profiles.

Value: `ProfileList`


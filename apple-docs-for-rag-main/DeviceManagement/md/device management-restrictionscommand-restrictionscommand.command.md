

- Device Management
- RestrictionsCommand
-  RestrictionsCommand.Command 

Device Management Command

# RestrictionsCommand.Command

The request dictionary to get a list of restrictions on a device.

iOS 4.0+iPadOS 4.0+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object RestrictionsCommand.Command
```

## Properties

`ProfileRestrictions`

`boolean`

If `true`, the device reports restrictions from each profile. This value is available in iOS 4 and later, and tvOS 6.1 and later.

Default: `false`

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get a list of restrictions on a device.

Value: `Restrictions`


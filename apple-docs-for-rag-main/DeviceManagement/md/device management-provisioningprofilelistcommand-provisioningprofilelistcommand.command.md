

- Device Management
- ProvisioningProfileListCommand
-  ProvisioningProfileListCommand.Command 

Device Management Command

# ProvisioningProfileListCommand.Command

The request dictionary to get a list of installed provisioning profiles.

iOS 4.0+iPadOS 4.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ProvisioningProfileListCommand.Command
```

## Properties

`ManagedOnly`

`boolean`

If `true`, only include profiles that MDM has installed. For user enrollments, the device ignores this key and always limits the results to managed profiles. This value is available in iOS 13 and later, and tvOS 13 and later.

Default: `false`

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get a list of installed provisioning profiles.

Value: `ProvisioningProfileList`


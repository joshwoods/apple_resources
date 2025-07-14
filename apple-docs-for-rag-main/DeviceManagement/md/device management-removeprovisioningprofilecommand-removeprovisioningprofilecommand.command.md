

- Device Management
- RemoveProvisioningProfileCommand
-  RemoveProvisioningProfileCommand.Command 

Device Management Command

# RemoveProvisioningProfileCommand.Command

The request dictionary to remove a profile.

iOS 4.0+iPadOS 4.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object RemoveProvisioningProfileCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to remove a provisioning profile.

Value: `RemoveProvisioningProfile`

`UUID`

`string`

 (Required) 

The unique identifier of the provisioning profile to remove.


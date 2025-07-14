

- Device Management
- InstallProvisioningProfileCommand
-  InstallProvisioningProfileCommand.Command 

Device Management Command

# InstallProvisioningProfileCommand.Command

The request dictionary to install a provisioning profile.

iOS 4.0+iPadOS 4.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstallProvisioningProfileCommand.Command
```

## Properties

`ProvisioningProfile`

`data`

 (Required) 

The provisioning profile.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to install a provisioning profile.

Value: `InstallProvisioningProfile`


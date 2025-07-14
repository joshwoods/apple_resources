

- Device Management
- ValidateApplicationsCommand
-  ValidateApplicationsCommand.Command 

Device Management Command

# ValidateApplicationsCommand.Command

The request dictionary to validate provisioning profiles for enterprise apps.

iOS 9.2+iPadOS 9.2+tvOS 10.2+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ValidateApplicationsCommand.Command
```

## Properties

`Identifiers`

`[string]`

The bundle identifiers of the enterprise apps to include for validation of associated provisioning profiles, if you choose to provide them. Otherwise, validation occurs for the provisioning profiles for the installed managed apps.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to validate app provisioning profiles.

Value: `ValidateApplications`


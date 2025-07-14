

- Device Management
- ContentCachingInformationCommand
-  ContentCachingInformationCommand.Command 

Device Management Command

# ContentCachingInformationCommand.Command

The command to get the status of the content caches on a device.

macOS 10.15.4+Device Assignment ServicesVPP License Management

``` source
object ContentCachingInformationCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the devce must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get the status of the content caches on a device.

Value: `ContentCachingInformation`


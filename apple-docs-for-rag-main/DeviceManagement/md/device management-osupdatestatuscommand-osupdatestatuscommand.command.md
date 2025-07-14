

- Device Management
- OSUpdateStatusCommand
-  OSUpdateStatusCommand.Command 

Device Management Command

# OSUpdateStatusCommand.Command

The request dictionary to get the status of operating-system updates.

iOS 9.0+iPadOS 9.0+macOS 10.11.5+tvOS 12.0+Device Assignment ServicesVPP License Management

``` source
object OSUpdateStatusCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get the status of operating-system updates.

Value: `OSUpdateStatus`


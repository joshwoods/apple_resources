

- Device Management
- AvailableOSUpdatesCommand
-  AvailableOSUpdatesCommand.Command 

Device Management Command

# AvailableOSUpdatesCommand.Command

The request dictionary to get a list of available operating-system updates.

iOS 9.0+iPadOS 9.0+macOS 10.11+tvOS 12.0+Device Assignment ServicesVPP License Management

``` source
object AvailableOSUpdatesCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get a list of available operating-system updates.

Value: `AvailableOSUpdates`


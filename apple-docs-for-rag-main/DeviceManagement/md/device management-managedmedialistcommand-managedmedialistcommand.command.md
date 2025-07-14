

- Device Management
- ManagedMediaListCommand
-  ManagedMediaListCommand.Command 

Device Management Command

# ManagedMediaListCommand.Command

The request dictionary to get a list of managed books.

iOS 8.0+iPadOS 8.0+Device Assignment ServicesVPP License Management

``` source
object ManagedMediaListCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get a list of managed books.

Value: `ManagedMediaList`


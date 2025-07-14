

- Device Management
- RequestUnlockTokenCommand
-  RequestUnlockTokenCommand.Command 

Device Management Command

# RequestUnlockTokenCommand.Command

The request dictionary to request an unlock token from a device.

iOS 5.0–6.1.6DeprecatediPadOS 5.0–6.1.6DeprecatedDevice Assignment ServicesVPP License Management

``` source
object RequestUnlockTokenCommand.Command
```

## Properties

`RequestRequiresNetworkTether`

`boolean`

Deprecated 

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

Deprecated   (Required) 

The request type to request an unlock token from a device.

Value: `RequestUnlockToken`


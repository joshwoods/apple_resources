

- Device Management
-  SetBootstrapTokenRequest 

Device Management Command

# SetBootstrapTokenRequest

The request object used to set the bootstrap token.

macOS 10.15+Device Assignment ServicesVPP License Management

``` source
object SetBootstrapTokenRequest
```

## Properties

`AwaitingConfiguration`

`boolean`

If `true`, the device is awaiting a DeviceConfigured MDM command before proceeding through Setup Assistant.

Default: `false`

`BootstrapToken`

`data`

The device’s bootstrap token data. If this field is missing or zero length, the bootstrap token should be removed for this device.

`MessageType`

`string`

 (Required) 

The message type, which must have a value of `SetBootstrapToken`.

Value: `SetBootstrapToken`


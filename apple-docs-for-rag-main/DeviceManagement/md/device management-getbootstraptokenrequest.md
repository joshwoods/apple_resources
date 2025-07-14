

- Device Management
-  GetBootstrapTokenRequest 

Device Management Command

# GetBootstrapTokenRequest

The request object used to get the bootstrap token.

macOS 10.15+Device Assignment ServicesVPP License Management

``` source
object GetBootstrapTokenRequest
```

## Properties

`AwaitingConfiguration`

`boolean`

If `true`, the device is awaiting a DeviceConfigured MDM command before proceeding through Setup Assistant.

Default: `false`

`MessageType`

`string`

 (Required) 

The message type, which must have a value of `GetBootstrapToken`.

Value: `GetBootstrapToken`

## See Also

### Request and Response

object GetBootstrapTokenResponse

The response that contains the bootstrap token.


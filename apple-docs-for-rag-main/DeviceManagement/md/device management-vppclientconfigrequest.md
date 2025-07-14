

- Device Management
-  VppClientConfigRequest 

Object

# VppClientConfigRequest

The request for the client configuration.

Device Assignment ServicesVPP License Management

``` source
object VppClientConfigRequest
```

## Properties

`clientContext`

`string`

Any JSON string under 256 bytes. The server stores the value of this field, and this value is returned in all responses. To clear the field’s value, provide an empty string as the input value (””).

See Protecting Your VPP Account for more information.

`notificationToken`

`string`

The token to use when sending notifications through `notificationURL`.

`sToken`

`string`

 (Required) 

The authentication token. For more information, see Authentication.

## See Also

### Request and Response

object VppClientConfigResponse

The response that contains the client configuration.


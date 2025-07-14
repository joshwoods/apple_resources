

- Device Management
-  ActivationLockRequest 

Object

# ActivationLockRequest

Request enabling activation lock for a device.

Device Assignment ServicesVPP License Management

``` source
object ActivationLockRequest
```

## Properties

`device`

`string`

Serial number of the device (required).

`escrow_key`

`string`

Escrow key (optional). If the escrow key is not provided, the device will be locked to the person who created the MDM server in the portal. For information about creating an escrow key see Creating and Using Bypass Codes.

`lost_message`

`string`

Lost message to be displayed on the device (optional).

## See Also

### Request and Response

object ActivationLockStatusResponse

The response to a request for activation lock.


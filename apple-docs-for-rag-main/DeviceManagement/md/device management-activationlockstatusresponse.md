

- Device Management
-  ActivationLockStatusResponse 

Object

# ActivationLockStatusResponse

The response to a request for activation lock.

Device Assignment ServicesVPP License Management

``` source
object ActivationLockStatusResponse
```

## Properties

`response_status`

`string`

\- `SUCCESS`: The device was successfully locked.

- `NOT_ACCESSIBLE:` The device with this serial number is not accessible by this user.

- `ORG_NOT_SUPPORTED:` The device with this serial number is not supported because it is not present in the new program.

- `DEVICE_NOT_SUPPORTED:` The device type is not supported.

- `DEVICE_ALREADY_LOCKED:` The device is already locked by someone.

- `FAILED:` Activation lock of the device failed for unexpected reason. If retry fails, the client should contact Apple support.

`serial_number`

`string`

Serial number of the device.

## See Also

### Request and Response

object ActivationLockRequest

Request enabling activation lock for a device.


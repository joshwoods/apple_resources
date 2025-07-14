

- Device Management
- DefineProfileResponse
-  DefineProfileResponse.Devices 

Object

# DefineProfileResponse.Devices

A dictionary containing device information.

Device Assignment ServicesVPP License Management

``` source
object DefineProfileResponse.Devices
```

## Properties

`Any Key`

`string`

Each key in this dictionary is the serial number of a device in the original request. Each value is one of the following strings:

- `SUCCESS`: The profile was mapped to the device.

- `NOT_ACCESSIBLE`: A device with the specified serial number was not accessible by this server.

- `FAILED`: Assigning the profile failed for an unexpected reason. If three retries fail, the user should contact Apple support.

## See Also

### Request and Response

object DefineProfileResponse

The response to defining a profile.




- Device Management
-  DefineProfileResponse 

Object

# DefineProfileResponse

The response to defining a profile.

Device Assignment ServicesVPP License Management

``` source
object DefineProfileResponse
```

## Properties

`devices`

DefineProfileResponse.Devices

A dictionary of devices. Each key in this dictionary is the serial number of a device in the original request. Each value is one of the following strings:

- `SUCCESS`: The profile was mapped to the device.

- `NOT_ACCESSIBLE`: A device with the specified serial number was not accessible by this server.

- `FAILED`: Assigning the profile failed for an unexpected reason. If three retries fail, the user should contact Apple support.

`profile_uuid`

`string`

The unique identifier for a profile.

## Topics

### Objects

object DefineProfileResponse.Devices

A dictionary containing device information.

## See Also

### Request and Response

object DefineProfileResponse.Devices

A dictionary containing device information.


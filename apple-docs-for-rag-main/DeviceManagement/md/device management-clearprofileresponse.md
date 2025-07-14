

- Device Management
-  ClearProfileResponse 

Object

# ClearProfileResponse

The response after removing a profile from devices.

Device Assignment ServicesVPP License Management

``` source
object ClearProfileResponse
```

## Properties

`devices`

ClearProfileResponse.Devices

A dictionary of devices. Each key in this dictionary is the serial number of a device in the original request. Each value is one of the following strings:

- `SUCCESS`: The profile was mapped to the device.

- `NOT_ACCESSIBLE`: A device with the specified serial number was not accessible by this server.

- `FAILED`: Assigning the profile failed for an unexpected reason. If three retries fail, the user should contact Apple support.

## Topics

### Objects

object ClearProfileResponse.Devices

A dictionary of devices with the status of their profile removal request.

## See Also

### Request and Response

object ClearProfileRequest

The request used to remove a profile from devices.

object ClearProfileResponse.Devices

A dictionary of devices with the status of their profile removal request.




- Device Management
-  DeviceStatusResponse 

Object

# DeviceStatusResponse

The request to get the status of a set of devices.

Device Assignment ServicesVPP License Management

``` source
object DeviceStatusResponse
```

## Properties

`devices`

DeviceStatusResponse.Devices

A dictionary of devices. Each key in this dictionary is the serial number of a device in the original request. Each value is one of the following values:

- `SUCCESS`: The device was successfully disowned.

- `NOT_ACCESSIBLE`: The device with the specified ID was not accessible by this MDM server.

- `FAILED`: Disowning the device failed for an unexpected reason. If three retries fail, the user should contact Apple support.

If no devices were provided in the original request, this dictionary may be absent.

## Topics

### Objects

object DeviceStatusResponse.Devices

A dictionary of devices with their status.

## See Also

### Response

object DeviceStatusResponse.Devices

A dictionary of devices with their status.


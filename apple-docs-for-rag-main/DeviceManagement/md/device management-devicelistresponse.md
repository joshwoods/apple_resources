

- Device Management
-  DeviceListResponse 

Object

# DeviceListResponse

The response that contains a list of devices.

Device Assignment ServicesVPP License Management

``` source
object DeviceListResponse
```

## Properties

`devices`

DeviceListResponse.Devices

A dictionary of devices. Each key in this dictionary is the serial number of a device in the original request. Each value is one of the following values:

- `SUCCESS`: Device was successfully disowned.

- `NOT_ACCESSIBLE`: A device with the specified ID was not accessible by this MDM server.

- `FAILED`: Disowning the device failed for an unexpected reason. If three retries fail, the user should contact Apple support.

If no devices were provided in the original request, this dictionary may be absent.

## Topics

### Objects

object DeviceListResponse.Devices

A dictionary of devices, with their serial numbers.

## See Also

### Request and Response

object DeviceListRequest

The request for a list of devices.

object DeviceListResponse.Devices

A dictionary of devices, with their serial numbers.


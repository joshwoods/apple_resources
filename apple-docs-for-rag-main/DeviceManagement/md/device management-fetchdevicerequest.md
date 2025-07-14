

- Device Management
-  FetchDeviceRequest 

Object

# FetchDeviceRequest

The request for a list of devices.

Device Assignment ServicesVPP License Management

``` source
object FetchDeviceRequest
```

## Properties

`cursor`

`string`

A hex string that represents the starting position for a request. Use this to retrieve the list of devices that have been added or removed since a previous request. The string can be up to 1000 characters. On the initial request, this should be omitted.

`limit`

`int32`

The maximum number of entries to return. Optional.

Default: `100`

Maximum: `1000`

## See Also

### Request and Response

object FetchDeviceResponse

The response that contains a list of devices.


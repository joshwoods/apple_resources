

- Device Management
-  SyncDeviceRequest 

Object

# SyncDeviceRequest

The request to sync the list of devices.

Device Assignment ServicesVPP License Management

``` source
object SyncDeviceRequest
```

## Properties

`cursor`

`string`

A hex string that represents the starting position for a request. Use this to retrieve the list of devices that have been added or removed since a previous request. The string can be up to 1000 characters.

`limit`

`int32`

The maximum number of entries to return. Optional.

Default: `100`

Maximum: `1000`


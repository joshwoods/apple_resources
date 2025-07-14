

- Device Management
-  ClearProfileRequest 

Object

# ClearProfileRequest

The request used to remove a profile from devices.

Device Assignment ServicesVPP License Management

``` source
object ClearProfileRequest
```

## Properties

`devices`

`[string]`

An array of strings containing device serial numbers.

`profile_uuid`

`string`

The unique identifier for a profile.

## See Also

### Request and Response

object ClearProfileResponse

The response after removing a profile from devices.

object ClearProfileResponse.Devices

A dictionary of devices with the status of their profile removal request.


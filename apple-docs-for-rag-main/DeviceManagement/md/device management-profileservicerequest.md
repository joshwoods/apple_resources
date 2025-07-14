

- Device Management
-  ProfileServiceRequest 

Object

# ProfileServiceRequest

The request for assigning a profile to a set of devices.

Device Assignment ServicesVPP License Management

``` source
object ProfileServiceRequest
```

## Properties

`devices`

`[string]`

Array of strings that contains device serial numbers.

`profile_uuid`

`string`

The unique identifier for a profile.

## See Also

### Request and Response

object AssignProfileResponse

The response to assigning a profile to a set of devices.

object AssignProfileResponse.Devices

A dictionary of device serial numbers mapped to the status of their profile assignment.


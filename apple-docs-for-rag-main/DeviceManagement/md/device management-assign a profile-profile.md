

- Device Management
-  Assign a Profile 

Web Service Endpoint

# Assign a Profile

Assign a profile to a list of devices.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/profile/devices
```

## HTTP Body

ProfileServiceRequest

The request for assigning a profile to a set of devices.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AssignProfileResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

- `DEVICE_ID_REQUIRED`: The request did not contain any device IDs.

- `PROFILE_UUID_REQUIRED`: The request did not contain a profile ID.

- `USER_AGENT_INVALID:` The `User-Agent` header is invalid.

- `USER_AGENT_MISSING:` The `User-Agent` header is missing or has no assigned value.

` 404 ``Not Found`

`Not Found`

The profile with the specified UUID could not be found.

## Discussion

To avoid performance issues, limit requests to 1000 devices at a time.

## Topics

### Request and Response

object ProfileServiceRequest

The request for assigning a profile to a set of devices.

object AssignProfileResponse

The response to assigning a profile to a set of devices.

object AssignProfileResponse.Devices

A dictionary of device serial numbers mapped to the status of their profile assignment.

## See Also

### Profile Management

Define a Profile

Define a profile that can be distributed to the devices in your organization.

Get a Profile

Get details about a profile.

Remove a Profile

Remove a profile from a list of devices.


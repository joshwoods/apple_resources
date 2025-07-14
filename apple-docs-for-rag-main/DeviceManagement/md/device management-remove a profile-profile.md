

- Device Management
-  Remove a Profile 

Web Service Endpoint

# Remove a Profile

Remove a profile from a list of devices.

Device Assignment ServicesVPP License Management

## URL

``` source
DELETE https://mdmenrollment.apple.com/profile/devices
```

## HTTP Body

ClearProfileRequest

The request used to remove a profile from devices.

Content-Type: application/json

## Response Codes

` 200 ``OK`

ClearProfileResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

- `DEVICE_ID_REQUIRED`: The request did not contain any device IDs.

- `USER_AGENT_INVALID:` The `User-Agent` header is invalid.

- `USER_AGENT_MISSING:` The `User-Agent` header is missing or has no assigned value.

## Discussion

After this call, the devices in the list will have no profiles associated with them. However, if those devices have already obtained the profile, this has no effect until the device is wiped and activated again.

## Topics

### Request and Response

object ClearProfileRequest

The request used to remove a profile from devices.

object ClearProfileResponse

The response after removing a profile from devices.

object ClearProfileResponse.Devices

A dictionary of devices with the status of their profile removal request.

## See Also

### Profile Management

Define a Profile

Define a profile that can be distributed to the devices in your organization.

Get a Profile

Get details about a profile.

Assign a Profile

Assign a profile to a list of devices.


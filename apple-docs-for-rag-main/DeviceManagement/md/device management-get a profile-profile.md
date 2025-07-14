

- Device Management
-  Get a Profile 

Web Service Endpoint

# Get a Profile

Get details about a profile.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://mdmenrollment.apple.com/profile
```

## Query Parameters

`profile_uuid`

`string`

 (Required) 

The unique identifier for a profile.

## Response Codes

` 200 ``OK`

Profile

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

- `PROFILE_UUID_REQUIRED`: The request did not contain a profile UUID.

- `NOT_FOUND`: The requested profile UUID doesn’t match a known profile.

- `USER_AGENT_INVALID:` The `User-Agent` header is invalid.

- `USER_AGENT_MISSING:` The `User-Agent` header is missing or has no assigned value.

## See Also

### Profile Management

Define a Profile

Define a profile that can be distributed to the devices in your organization.

Assign a Profile

Assign a profile to a list of devices.

Remove a Profile

Remove a profile from a list of devices.


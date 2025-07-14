

- Device Management
-  Get Beta Enrollment Tokens 

Web Service Endpoint

# Get Beta Enrollment Tokens

Retrieves the beta enrollment tokens available for the organization.

Device Assignment ServicesVPP License Management

## URL

``` source
GET https://mdmenrollment.apple.com/os-beta-enrollment/tokens
```

## Response Codes

` 200 ``OK`

GetSeedBuildTokenResponse

`OK`

Content-Type: application/json

` 403 ``APPLE_SEED_FOR_IT_TURNED_OFF`

`APPLE_SEED_FOR_IT_TURNED_OFF`

No access - your organization doesn’t allow beta access.

## Topics

### Response

object GetSeedBuildTokenResponse

Provides a list of beta enrollment tokens available for the given organization.

object SeedBuildToken

Describes a beta enrollment token available for the given organization.

## See Also

### Device Management

Activation Lock a Device

Enable activation lock on a remote device.

Get Device Details

Get the details on a set of devices.

Get a List of Devices

Get a list of devices that are managed by the server.

Sync the List of Devices

Get updates about the list of devices the server manages.

Disown Devices

Notify Apple’s servers that your organization no longer owns the specified devices.


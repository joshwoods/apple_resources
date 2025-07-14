

- Device Management
-  Get a List of Devices 

Web Service Endpoint

# Get a List of Devices

Get a list of devices that are managed by the server.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/server/devices
```

## HTTP Body

FetchDeviceRequest

The request for a list of devices.

Content-Type: application/json

## Response Codes

` 200 ``OK`

FetchDeviceResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

- `INVALID_CURSOR`: An invalid cursor value was provided.

- `EXHAUSTED_CURSOR`: The cursor had returned all devices in previous calls.

- `USER_AGENT_INVALID:` The `User-Agent` header is invalid.

- `USER_AGENT_MISSING:` The `User-Agent` header is missing or has no assigned value.

## Discussion

This request fetches a list of all devices that are assigned to this MDM server at the time of the request. This service should be used for loading an initial list of devices into the MDM server’s data store. Once the list of devices is loaded, Sync the List of Devices to update the list.

This request provides a limited number of entries per request, using cursors to provide position information across requests.

## Topics

### Request and Response

object FetchDeviceRequest

The request for a list of devices.

object FetchDeviceResponse

The response that contains a list of devices.

## See Also

### Device Management

Activation Lock a Device

Enable activation lock on a remote device.

Get Device Details

Get the details on a set of devices.

Sync the List of Devices

Get updates about the list of devices the server manages.

Disown Devices

Notify Apple’s servers that your organization no longer owns the specified devices.

Get Beta Enrollment Tokens

Retrieves the beta enrollment tokens available for the organization.


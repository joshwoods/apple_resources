

- Device Management
-  Get Device Details 

Web Service Endpoint

# Get Device Details

Get the details on a set of devices.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/devices
```

## HTTP Body

DeviceListRequest

The request for a list of devices.

Content-Type: application/json

## Response Codes

` 200 ``OK`

DeviceListResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

- `DEVICE_ID_REQUIRED`: No device IDs (serial numbers) were provided.

- `USER_AGENT_INVALID:` The `User-Agent` header is invalid.

- `USER_AGENT_MISSING:` The `User-Agent` header is missing or has no assigned value.

## Discussion

## Topics

### Request and Response

object DeviceListRequest

The request for a list of devices.

object DeviceListResponse

The response that contains a list of devices.

object DeviceListResponse.Devices

A dictionary of devices, with their serial numbers.

## See Also

### Device Management

Activation Lock a Device

Enable activation lock on a remote device.

Get a List of Devices

Get a list of devices that are managed by the server.

Sync the List of Devices

Get updates about the list of devices the server manages.

Disown Devices

Notify Apple’s servers that your organization no longer owns the specified devices.

Get Beta Enrollment Tokens

Retrieves the beta enrollment tokens available for the organization.


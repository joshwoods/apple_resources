

- Device Management
-  Disown Devices 

Web Service Endpoint

# Disown Devices

Notify Apple’s servers that your organization no longer owns the specified devices.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/devices/disown
```

## HTTP Body

DeviceListRequest

The request for a list of devices.

Content-Type: application/json

## Response Codes

` 200 ``OK`

DeviceStatusResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

- `DEVICE_ID_REQUIRED`: The request did not contain any devices.

- `USER_AGENT_INVALID:` The `User-Agent` header is invalid.

- `USER_AGENT_MISSING:` The `User-Agent` header is missing or has no assigned value.

## Topics

### Response

object DeviceStatusResponse

The request to get the status of a set of devices.

object DeviceStatusResponse.Devices

A dictionary of devices with their status.

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

Get Beta Enrollment Tokens

Retrieves the beta enrollment tokens available for the organization.


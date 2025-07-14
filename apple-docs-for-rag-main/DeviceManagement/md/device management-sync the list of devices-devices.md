

- Device Management
-  Sync the List of Devices 

Web Service Endpoint

# Sync the List of Devices

Get updates about the list of devices the server manages.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/devices/sync
```

## HTTP Body

SyncDeviceRequest

The request to sync the list of devices.

Content-Type: application/json

## Response Codes

` 200 ``OK`

FetchDeviceResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

- `CURSOR_REQUIRED`: `The cursor value was not provided in the request body.`

- `INVALID_CURSOR`: An invalid cursor value was provided.

- `EXHAUSTED_CURSOR`: The cursor had returned all devices in previous calls.

- `EXPIRED_CURSOR`: The provided cursor is older than 7 days.

- `USER_AGENT_INVALID:` The `User-Agent` header is invalid.

- `USER_AGENT_MISSING:` The `User-Agent` header is missing or has no assigned value.

## Discussion

The sync service depends on a cursor returned by the fetch device service. It returns a list of all modifications (additions or deletions) since the specified cursor. The cursor passed to this endpoint should not be older than 7 days.

This service may return the same device more than once. You must resolve duplicates by matching on the device serial number and the `op_type` and `op_date` fields. The record with the latest `op_date` indicates the last known state of the device in DEP.

## Topics

### Request

object SyncDeviceRequest

The request to sync the list of devices.

## See Also

### Device Management

Activation Lock a Device

Enable activation lock on a remote device.

Get Device Details

Get the details on a set of devices.

Get a List of Devices

Get a list of devices that are managed by the server.

Disown Devices

Notify Apple’s servers that your organization no longer owns the specified devices.

Get Beta Enrollment Tokens

Retrieves the beta enrollment tokens available for the organization.


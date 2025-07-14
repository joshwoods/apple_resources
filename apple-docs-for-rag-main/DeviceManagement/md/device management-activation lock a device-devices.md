

- Device Management
-  Activation Lock a Device 

Web Service Endpoint

# Activation Lock a Device

Enable activation lock on a remote device.

Device Assignment ServicesVPP License Management

## URL

``` source
POST https://mdmenrollment.apple.com/device/activationlock
```

## HTTP Body

ActivationLockRequest

Request enabling activation lock for a device.

Content-Type: application/json

## Response Codes

` 200 ``OK`

ActivationLockStatusResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

- `MALFORMED_REQUEST_BODY`: The request body is malformed.

- `USER_AGENT_INVALID:` The `User-Agent` header is invalid.

- `USER_AGENT_MISSING:` The `User-Agent` header is missing or has no assigned value.

` 401 ``Unauthorized`

`Unauthorized`

The token has expired. The client should retry with a new auth token.

` 403 ``Forbidden`

`Forbidden`

The auth token is invalid.

## Discussion

Find My iPhone Activation Lock is a feature of iCloud and Automated Device Enrollment that makes it harder for anyone to use or resell a lost or stolen iOS device. Activation Lock is a feature of iCloud, and MDM has the ability to allow users to enable the feature on Supervised devices.

There are two ways to manage Activation Lock: the Activation Lock request is available for devices that appear in the Apple School Manager portal or Apple Business Manager portal, or the Find My approach. Whichever method is the first to enable Activation Lock takes precedence.

## Topics

### Request and Response

object ActivationLockRequest

Request enabling activation lock for a device.

object ActivationLockStatusResponse

The response to a request for activation lock.

### Bypass Codes

Creating and Using Bypass Codes

Maintain the bypass code parameters for disabling Activation Lock.

## See Also

### Device Management

Get Device Details

Get the details on a set of devices.

Get a List of Devices

Get a list of devices that are managed by the server.

Sync the List of Devices

Get updates about the list of devices the server manages.

Disown Devices

Notify Apple’s servers that your organization no longer owns the specified devices.

Get Beta Enrollment Tokens

Retrieves the beta enrollment tokens available for the organization.


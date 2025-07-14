

- Device Management
-  ClientConfigRequest 

Object

# ClientConfigRequest

The request for the client configuration.

Device Assignment ServicesVPP License Management

``` source
object ClientConfigRequest
```

## Properties

`notificationTypes`

`[string]`

The complete set of notification types to which MDM subscribes.

Possible Values: `ASSET_MANAGEMENT, USER_MANAGEMENT, USER_ASSOCIATED, ASSET_COUNT`

`notificationUrl`

`string`

The URL to which subscribed notifications POST. This URL should only include a host and path.

`mdmInfo`

MdmInfo

This value is returned by the server on all subsequent responses, and MDM uses it to ensure that no other MDM manages the same organization.

`notificationAuthToken`

`string`

The bearer token that the server provides in the Authorization header of notifications. This is a shared secret between you and the server to verify that incoming notifications are from Apple.

## Mentioned in 

Subscribing to Notifications

Upgrading to the new App and Book Management API

## Topics

### Objects and Data Types

object MdmInfo

Information about the MDM client.

## See Also

### Request and Response

object ClientConfigResponse

The response that contains the client configuration.

object ErrorResponse

The response that contains the error that occurs.


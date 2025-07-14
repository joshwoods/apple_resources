

- Device Management
-  ServiceConfigResponse 

Object

# ServiceConfigResponse

The response that contains the service configuration.

Device Assignment ServicesVPP License Management

``` source
object ServiceConfigResponse
```

## Properties

`errorCodes`

`[`ResponseErrorCode`]`

The list of possible error numbers and their human-readable explanations.

`limits`

ServiceConfigResponse.Limits

The set of current request limits.

The MDM server checks these values every 5 minutes because they might change without notice.

`notificationTypes`

`[string]`

The set of supported notification types.

`urls`

ServiceConfigResponse.Urls

The set of current service URLs.

The MDM server checks these values every 5 minutes because they might change without notice.

## Topics

### Objects and Data Types

object ResponseErrorCode

An error code.

object ServiceConfigResponse.Limits

The mutable limits for request sizes.

object ServiceConfigResponse.Urls

The URLs for all endpoints.

## See Also

### Response

object ErrorResponse

The response that contains the error that occurs.


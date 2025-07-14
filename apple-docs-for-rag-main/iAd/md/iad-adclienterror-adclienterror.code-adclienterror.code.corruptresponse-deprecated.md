

- iAd
- ADClientError
- ADClientError.Code
-  ADClientError.Code.corruptResponse Deprecated

Case

# ADClientError.Code.corruptResponse

The response from the attribution server is corrupt.

``` source
case corruptResponse
```

Deprecated

This has been replaced by functionality in AdServices.framework's AAAttribution class.

## See Also

### Error Codes

case requestClientError

The response from the attribution server has an HTTP 4xx status code.

Deprecated

case requestNetworkError

The communication with the attribution server has a network error.

Deprecated

case requestServerError

The response from the attribution server has an HTTP 5xx status code.

Deprecated

case trackingRestrictedOrDenied

The user has a restricted status or has denied tracking for the calling app.

Deprecated

case missingData

The downloaded app has a payload without enough data to perform an attribution check.

Deprecated

case unsupportedPlatform

The system doesn’t support the platform for the attribution API call.

Deprecated

case unknown

The response from the attribution server has an unknown error.

Deprecated

static var limitAdTracking: ADClientError.CodeDeprecated


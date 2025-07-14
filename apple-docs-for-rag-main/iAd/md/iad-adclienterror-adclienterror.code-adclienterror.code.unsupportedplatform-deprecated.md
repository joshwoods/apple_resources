

- iAd
- ADClientError
- ADClientError.Code
-  ADClientError.Code.unsupportedPlatform Deprecated

Case

# ADClientError.Code.unsupportedPlatform

The system doesn’t support the platform for the attribution API call.

``` source
case unsupportedPlatform
```

Deprecated

This has been replaced by functionality in AdServices.framework's AAAttribution class.

## Discussion

The Search Ads Attribution API only supports iOS and iPadOS.

## See Also

### Error Codes

case corruptResponse

The response from the attribution server is corrupt.

Deprecated

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

case unknown

The response from the attribution server has an unknown error.

Deprecated

static var limitAdTracking: ADClientError.CodeDeprecated


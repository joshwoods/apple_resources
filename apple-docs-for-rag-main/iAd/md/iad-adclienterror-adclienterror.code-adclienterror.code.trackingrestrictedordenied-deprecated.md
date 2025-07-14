

- iAd
- ADClientError
- ADClientError.Code
-  ADClientError.Code.trackingRestrictedOrDenied Deprecated

Case

# ADClientError.Code.trackingRestrictedOrDenied

The user has a restricted status or has denied tracking for the calling app.

``` source
case trackingRestrictedOrDenied
```

Deprecated

This has been replaced by functionality in AdServices.framework's AAAttribution class.

## Discussion

Restricted status occurs in the following conditions:

- The registered user of the App Store Connect account is a minor.

- The device is in educational mode.

- The account is a managed account.

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


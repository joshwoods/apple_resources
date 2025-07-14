

- iAd
- ADClientError
- ADClientError.Code
-  ADClientError.Code.unknown Deprecated

Case

# ADClientError.Code.unknown

The response from the attribution server has an unknown error.

``` source
case unknown
```

Deprecated

ADClientErrorUnknown is not used and never returned.

## Discussion

Wait a few seconds and try again. When you’ve successfully retrieved your attribution data, you don’t need to poll for data again. The values you retrieve don’t change.

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

case unsupportedPlatform

The system doesn’t support the platform for the attribution API call.

Deprecated

static var limitAdTracking: ADClientError.CodeDeprecated


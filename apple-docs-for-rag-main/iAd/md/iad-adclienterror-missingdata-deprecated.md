

- iAd
- ADClientError
-  missingData Deprecated

Type Property

# missingData

The downloaded app received a payload lacking enough data to perform an attribution check.

``` source
static var missingData: ADClientError.Code { get }
```

Deprecated

This has been replaced by functionality in AdServices.framework's AAAttribution class.

## See Also

### Error Codes

static var corruptResponse: ADClientError.Code

The response received from the attribution server was corrupt.

Deprecated

static var requestClientError: ADClientError.Code

The response received from the attribution server had an HTTP 4xx status code.

Deprecated

static var requestNetworkError: ADClientError.Code

The communication with the attribution server had a network error.

Deprecated

static var requestServerError: ADClientError.Code

The response received from the attribution server had an HTTP 5xx status code.

Deprecated

static var trackingRestrictedOrDenied: ADClientError.Code

The user is restricted or has denied tracking for the calling application.

Deprecated

static var unsupportedPlatform: ADClientError.Code

The attribution API was called on an unsupported platform.

Deprecated

static var limitAdTracking: ADClientError.CodeDeprecated

static var unknown: ADClientError.CodeDeprecated

enum Code

The error codes that pass from the attribution response to the completion handler.

Deprecated


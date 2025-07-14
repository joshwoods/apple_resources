

- iAd
- ADClientError
-  ADClientError.Code Deprecated

Enumeration

# ADClientError.Code

The error codes that pass from the attribution response to the completion handler.

``` source
enum Code
```

Deprecated

This has been replaced by functionality in AdServices.framework's AAAttribution class.

## Overview

The group of error codes that pass from the attribution response to the completion handler block when you call the requestAttributionDetails(_:) method.

## Topics

### Error Codes

case corruptResponse

The response from the attribution server is corrupt.

case requestClientError

The response from the attribution server has an HTTP 4xx status code.

case requestNetworkError

The communication with the attribution server has a network error.

case requestServerError

The response from the attribution server has an HTTP 5xx status code.

case trackingRestrictedOrDenied

The user has a restricted status or has denied tracking for the calling app.

case missingData

The downloaded app has a payload without enough data to perform an attribution check.

case unsupportedPlatform

The system doesn’t support the platform for the attribution API call.

case unknown

The response from the attribution server has an unknown error.

static var limitAdTracking: ADClientError.Code

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Attribution Errors

let ADClientErrorDomain: String

The error domain that passes to the completion handler.

Deprecated

struct ADClientError

The group of error codes that pass from the attribution response to the completion handler block.

Deprecated


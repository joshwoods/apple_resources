

- CloudKit
- CKError
-  retryAfterSeconds 

Instance Property

# retryAfterSeconds

The number of seconds to wait before you retry the request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+

``` source
var retryAfterSeconds: Double? { get }
```

## Discussion

This property’s value is available only when the error’s `code` is serviceUnavailable or requestRateLimited.

The error’s `userInfo` dictionary contains the same value as this property. You can access it using the CKErrorRetryAfterKey key.


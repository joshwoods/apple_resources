

- AVFoundation
- AVContentKeyRequest
- AVContentKeyRequest.RetryReason
-  receivedResponseWithExpiredLease 

Type Property

# receivedResponseWithExpiredLease

A key response with an expired lease that was set on the previous content key request.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
static let receivedResponseWithExpiredLease: AVContentKeyRequest.RetryReason
```

## See Also

### Reasons for Content Key Request Retry

static let receivedObsoleteContentKey: AVContentKeyRequest.RetryReason

An obsolete key response that was set on the previous content key request.

static let timedOut: AVContentKeyRequest.RetryReason

A key response that wasn’t set soon enough.


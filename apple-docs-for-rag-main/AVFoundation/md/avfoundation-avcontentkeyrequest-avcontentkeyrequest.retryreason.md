

- AVFoundation
- AVContentKeyRequest
-  AVContentKeyRequest.RetryReason 

Structure

# AVContentKeyRequest.RetryReason

The reason for asking the client to retry a content key request.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
struct RetryReason
```

## Topics

### Reasons for Content Key Request Retry

static let receivedObsoleteContentKey: AVContentKeyRequest.RetryReason

An obsolete key response that was set on the previous content key request.

static let receivedResponseWithExpiredLease: AVContentKeyRequest.RetryReason

A key response with an expired lease that was set on the previous content key request.

static let timedOut: AVContentKeyRequest.RetryReason

A key response that wasn’t set soon enough.

### Initializers

init(rawValue: String)

Creates a retry reason with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting a Request

var contentKey: AVContentKey?

The generated content key.

var contentKeySpecifier: AVContentKeySpecifier

The requested content key specifier.

var options: [String : any Sendable]

A dictionary of options used to initialize key loading.


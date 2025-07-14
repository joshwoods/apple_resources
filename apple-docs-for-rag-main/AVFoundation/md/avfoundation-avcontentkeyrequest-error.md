

- AVFoundation
- AVContentKeyRequest
-  error 

Instance Property

# error

The error description for a failed key request.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
var error: (any Error)? { get }
```

## See Also

### Getting Content Key Request Properties

var identifier: (any Sendable)?

The identifier for the content key.

var canProvidePersistableContentKey: Bool

The content key request used to create a persistable content key or respond to a previous request with a persistable content key.

var initializationData: Data?

The data used to obtain a key response.

var renewsExpiringResponseData: Bool

A Boolean value that indicates whether the content key request renews previously provided response data.

var status: AVContentKeyRequest.Status

The current state of the content key request.

enum Status

The status for a content key request.




- AVFoundation
- AVContentKeyRequest
-  canProvidePersistableContentKey 

Instance Property

# canProvidePersistableContentKey

The content key request used to create a persistable content key or respond to a previous request with a persistable content key.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
var canProvidePersistableContentKey: Bool { get }
```

## Discussion

The value of this property is automatically set to `YES` when the receiver is provided to the content key session’s delegate via the contentKeySession(_:didProvide:) method. When this property is set to `YES`, the persistableContentKey(fromKeyVendorResponse:options:) method can be used to create a persistable content key from the response.

When this property is set to `NO` and there is a request for a persistable content key, send the respondByRequestingPersistableContentKeyRequest() method.

## See Also

### Getting Content Key Request Properties

var identifier: (any Sendable)?

The identifier for the content key.

var error: (any Error)?

The error description for a failed key request.

var initializationData: Data?

The data used to obtain a key response.

var renewsExpiringResponseData: Bool

A Boolean value that indicates whether the content key request renews previously provided response data.

var status: AVContentKeyRequest.Status

The current state of the content key request.

enum Status

The status for a content key request.


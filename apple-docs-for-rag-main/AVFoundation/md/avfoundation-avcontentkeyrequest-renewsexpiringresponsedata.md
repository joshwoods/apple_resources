

- AVFoundation
- AVContentKeyRequest
-  renewsExpiringResponseData 

Instance Property

# renewsExpiringResponseData

A Boolean value that indicates whether the content key request renews previously provided response data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var renewsExpiringResponseData: Bool { get }
```

## Discussion

The value of this property is `YES` if the request renews previously provided response data that is expiring or has already expired.

## See Also

### Getting Content Key Request Properties

var identifier: (any Sendable)?

The identifier for the content key.

var canProvidePersistableContentKey: Bool

The content key request used to create a persistable content key or respond to a previous request with a persistable content key.

var error: (any Error)?

The error description for a failed key request.

var initializationData: Data?

The data used to obtain a key response.

var status: AVContentKeyRequest.Status

The current state of the content key request.

enum Status

The status for a content key request.


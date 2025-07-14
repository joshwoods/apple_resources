

- CloudKit
- CKOperation
- CKOperation.Configuration
-  isLongLived 

Instance Property

# isLongLived

A Boolean value that indicates whether the operations that use this configuration are long-lived.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var isLongLived: Bool { get set }
```

## See Also

### Preparing a Configuration

var allowsCellularAccess: Bool

A Boolean value that indicates whether operations that use this configuration can send data over the cellular network.

var container: CKContainer?

The configuration’s container.

var qualityOfService: QualityOfService

The priority that the system uses when it allocates resources to the operations that use this configuration.

var timeoutIntervalForRequest: TimeInterval

The maximum amount of time that a request can take.

var timeoutIntervalForResource: TimeInterval

The maximum amount of time that a resource request can take.


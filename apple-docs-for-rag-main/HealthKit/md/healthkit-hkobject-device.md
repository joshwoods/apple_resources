

- HealthKit
- HKObject
-  device 

Instance Property

# device

The device that generated the data for this object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var device: HKDevice? { get }
```

## See Also

### Accessing Properties

var uuid: UUID

The universally unique identifier (UUID) for this HealthKit object.

var metadata: [String : Any]?

The metadata for this HealthKit object.

var sourceRevision: HKSourceRevision

The app or device that created this object.

var source: HKSource

A HealthKit source, representing the app or device that created this object.

Deprecated


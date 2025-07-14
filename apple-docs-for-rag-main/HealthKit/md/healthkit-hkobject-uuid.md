

- HealthKit
- HKObject
-  uuid 

Instance Property

# uuid

The universally unique identifier (UUID) for this HealthKit object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var uuid: UUID { get }
```

## Discussion

HealthKit assigns a UUID to the object when you create it. If you want to add your own unique ID, add it to the object’s metadata using the HKMetadataKeyExternalUUID key.

## See Also

### Accessing Properties

var metadata: [String : Any]?

The metadata for this HealthKit object.

var device: HKDevice?

The device that generated the data for this object.

var sourceRevision: HKSourceRevision

The app or device that created this object.

var source: HKSource

A HealthKit source, representing the app or device that created this object.

Deprecated


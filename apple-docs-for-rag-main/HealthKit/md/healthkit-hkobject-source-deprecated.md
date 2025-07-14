

- HealthKit
- HKObject
-  source Deprecated

Instance Property

# source

A HealthKit source, representing the app or device that created this object.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var source: HKSource { get }
```

Deprecated

This property is deprecated. Use sourceRevision instead.

## Discussion

The `source` property is only available on objects you have retrieved from the HealthKit store. When you create a new object, the source is set to `nil`. The system automatically sets the source property when you save the object to the HealthKit store. The source is then available the next time the object is retrieved from the store.

## See Also

### Accessing Properties

var uuid: UUID

The universally unique identifier (UUID) for this HealthKit object.

var metadata: [String : Any]?

The metadata for this HealthKit object.

var device: HKDevice?

The device that generated the data for this object.

var sourceRevision: HKSourceRevision

The app or device that created this object.


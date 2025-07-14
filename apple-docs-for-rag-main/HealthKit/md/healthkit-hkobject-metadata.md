

- HealthKit
- HKObject
-  metadata 

Instance Property

# metadata

The metadata for this HealthKit object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var metadata: [String : Any]? { get }
```

## Discussion

The metadata dictionary contains extra information describing this object. The dictionary’s keys are all NSString objects. The values can be NSString objects, NSNumber objects or NSDate objects. For a complete list of predefined metadata keys, see Metadata Keys.

Using predefined keys helps facilitate sharing data between apps; however, you are also encouraged to create your own, custom keys as needed to extend the HealthKit object’s capabilities.

You set an object’s metadata when you create the object by calling one of these methods (or a related method):

- init(type:quantity:start:end:metadata:)

- init(type:value:start:end:metadata:)

- init(type:start:end:objects:metadata:)

- init(activityType:start:end:duration:totalEnergyBurned:totalDistance:metadata:)

## See Also

### Accessing Properties

var uuid: UUID

The universally unique identifier (UUID) for this HealthKit object.

var device: HKDevice?

The device that generated the data for this object.

var sourceRevision: HKSourceRevision

The app or device that created this object.

var source: HKSource

A HealthKit source, representing the app or device that created this object.

Deprecated




- HealthKit
-  HKSeriesType 

Class

# HKSeriesType

A type that indicates the data stored in a series sample.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
class HKSeriesType
```

## Topics

### Accessing Series Types

class func workoutRoute() -> Self

Returns a series type object for workout routes.

class func heartbeat() -> Self

Returns a series type object for heartbeat data.

## Relationships

### Inherits From

- HKSampleType

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Related Documentation

class HKWorkoutRoute

A sample that contains a workout’s route data.

class HKWorkoutRouteBuilder

A builder object that incrementally constructs a workout route.

class HKWorkoutRouteQuery

A query to access the location data stored in a workout route.

### Object type subclasses

class HKCharacteristicType

A type that represents data that doesn’t typically change over time.

class HKQuantityType

A type that identifies samples that store numerical values.

class HKCategoryType

A type that identifies samples that contain a value from a small set of possible values.

class HKCorrelationType

A type that identifies samples that group multiple subsamples.

class HKActivitySummaryType

A type that identifies activity summary objects.

class HKAudiogramSampleType

A type that identifies samples that contain audiogram data.

class HKElectrocardiogramType

A type that identifies samples containing electrocardiogram data.

class HKClinicalType

A type that identifies samples that contain clinical record data.

class HKWorkoutType

A type that identifies samples that store information about a workout.

class HKObjectType

An abstract superclass with subclasses that identify a specific type of data for the HealthKit store.

class HKSampleType

An abstract superclass for all classes that identify a specific type of sample when working with the HealthKit store.


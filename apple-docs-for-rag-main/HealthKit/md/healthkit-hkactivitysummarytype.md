

- HealthKit
-  HKActivitySummaryType 

Class

# HKActivitySummaryType

A type that identifies activity summary objects.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.2+

``` source
class HKActivitySummaryType
```

## Overview

Use the activity summary type to request permission to read HKActivitySummary objects from the HealthKit store. To create an activity summary type, use the HKObjectType class’s activitySummaryType() convenience method.

Note

Although you can request permission to read HKActivitySummary objects, you can’t request permission to share them. For more information, see requestAuthorization(toShare:read:completion:).

The HKActivitySummaryType class is a concrete subclass of the HKObjectType class. Like many HealthKit classes, activity summary types aren’t extensible and you shouldn’t subclass them.

### Access and Modify Activity Summaries

Any workouts that you save to the HealthKit store may affect that day’s summary. For more information, see `Using Workout Samples`.

To query for activity summary objects, use an HKActivitySummaryQuery. You can also create your own HKActivitySummary objects (for example, to display in an HKActivityRingView), but you can’t save them to the HealthKit store.

## Relationships

### Inherits From

- HKObjectType

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

class HKActivitySummary

An object that contains the move, exercise, and stand data for a given day.

class HKActivitySummaryQuery

A query for reading activity summary objects from the HealthKit store.

class HKActivityRingView

A view that uses the Move, Exercise, and Stand activity rings to display data from a HealthKit activity summary object.

### Object type subclasses

class HKCharacteristicType

A type that represents data that doesn’t typically change over time.

class HKQuantityType

A type that identifies samples that store numerical values.

class HKCategoryType

A type that identifies samples that contain a value from a small set of possible values.

class HKCorrelationType

A type that identifies samples that group multiple subsamples.

class HKAudiogramSampleType

A type that identifies samples that contain audiogram data.

class HKElectrocardiogramType

A type that identifies samples containing electrocardiogram data.

class HKSeriesType

A type that indicates the data stored in a series sample.

class HKClinicalType

A type that identifies samples that contain clinical record data.

class HKWorkoutType

A type that identifies samples that store information about a workout.

class HKObjectType

An abstract superclass with subclasses that identify a specific type of data for the HealthKit store.

class HKSampleType

An abstract superclass for all classes that identify a specific type of sample when working with the HealthKit store.


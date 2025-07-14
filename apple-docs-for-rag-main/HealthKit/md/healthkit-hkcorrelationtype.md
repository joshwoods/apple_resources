

- HealthKit
-  HKCorrelationType 

Class

# HKCorrelationType

A type that identifies samples that group multiple subsamples.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKCorrelationType
```

## Overview

The HKCorrelationType class is a concrete subclass of the HKObjectType class. To create a correlation type instance, use the object type’s correlationType(forIdentifier:) conveniance method.

Use correlation types to:

- Request permission to read or write matching quantity samples.

- Create and share matching quantity samples.

- Query for matching quantity samples.

HealthKit provides two correlation types: blood pressure and food.

### Using Correlation Types

Like many HealthKit classes, correlation types are not extensible and should not be subclassed.

This class reuses the same instance whenever possible. Letting multiple queries share the same workout type helps reduce the overall memory usage.

## Topics

### Creating Correlation Types

convenience init(HKCorrelationTypeIdentifier)

Creates a correlation type using the provided identifier.

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

struct HKCorrelationTypeIdentifier

The identifiers that create correlation type objects.

class HKCorrelation

A sample that groups multiple related samples into a single entry.

### Object type subclasses

class HKCharacteristicType

A type that represents data that doesn’t typically change over time.

class HKQuantityType

A type that identifies samples that store numerical values.

class HKCategoryType

A type that identifies samples that contain a value from a small set of possible values.

class HKActivitySummaryType

A type that identifies activity summary objects.

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


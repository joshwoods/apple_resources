

- HealthKit
-  HKQuantityType 

Class

# HKQuantityType

A type that identifies samples that store numerical values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKQuantityType
```

## Mentioned in 

Saving data to HealthKit

## Overview

The HKQuantityType class is a concrete subclass of the HKObjectType class. To create a quantity type instance, use the object type’s quantityType(forIdentifier:) convenience method.

Use quantity types to:

- Request permission to read or write matching quantity samples.

- Create and share matching quantity samples.

- Query for matching quantity samples.

## Topics

### Creating Quantity Types

convenience init(HKQuantityTypeIdentifier)

Creates a quantity type using the provided identifier.

### Accessing Quantity Type Data

var aggregationStyle: HKQuantityAggregationStyle

The aggregation style for the given quantity type.

enum HKQuantityAggregationStyle

Constant values that describe how quantities can be aggregated over time.

func `is`(compatibleWith: HKUnit) -> Bool

Returns a Boolean value that indicates whether the quantity type is compatible with the given unit.

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

struct HKQuantityTypeIdentifier

The identifiers that create quantity type objects.

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

### Object type subclasses

class HKCharacteristicType

A type that represents data that doesn’t typically change over time.

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


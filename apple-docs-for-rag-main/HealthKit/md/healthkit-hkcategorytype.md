

- HealthKit
-  HKCategoryType 

Class

# HKCategoryType

A type that identifies samples that contain a value from a small set of possible values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKCategoryType
```

## Overview

The HKCategoryType class is a concrete subclass of the HKObjectType class. To create a category type instance, use the object type’s categoryType(forIdentifier:) convenience method.

Use category types to:

- Request permission to read or write matching quantity samples.

- Create and share matching quantity samples.

- Query for matching quantity samples.

## Topics

### Creating Category Types

convenience init(HKCategoryTypeIdentifier)

Creates a category type using the provided identifier.

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

struct HKCategoryTypeIdentifier

Identifiers for creating category types.

class HKCategorySample

A sample with values from a short list of possible values.

### Object type subclasses

class HKCharacteristicType

A type that represents data that doesn’t typically change over time.

class HKQuantityType

A type that identifies samples that store numerical values.

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


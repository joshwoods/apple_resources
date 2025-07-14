

- HealthKit
-  HKCharacteristicType 

Class

# HKCharacteristicType

A type that represents data that doesn’t typically change over time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKCharacteristicType
```

## Overview

The HKCharacteristicType class is a concrete subclass of the HKObjectType class. To create a characteristic type instance, use the object type’s characteristicType(forIdentifier:) convenience method.

Unlike the other object types, characteristic types cannot be used to create and save new HealthKit objects. Instead, users must enter and edit their characteristic data using the Health app. Similarly, you cannot create queries for characteristic types. Instead, use the HealthKit store to access the data (see Reading characteristic data).

HealthKit provides five characteristic types: biological sex, blood type, birthdate, Fitzpatrick skin type, and wheelchair use. These types are used only when asking for permission to read data from the HealthKit store.

## Topics

### Creating Characteristic Types

convenience init(HKCharacteristicTypeIdentifier)

Creates a characteristic type using the provided identifier.

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

struct HKCharacteristicTypeIdentifier

The identifiers that create characteristic type objects.

### Object type subclasses

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


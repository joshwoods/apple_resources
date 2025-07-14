

- HealthKit
-  HKElectrocardiogramType 

Class

# HKElectrocardiogramType

A type that identifies samples containing electrocardiogram data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class HKElectrocardiogramType
```

## Overview

The HKElectrocardiogramType class is a concrete subclass of the HKObjectType class. To create an electrocardiogram type instance, use the object type’s electrocardiogramType() convenience method.

Use the electrocardiogram type to:

- Request permission to read electrocardiogram samples

- Query for electrocardiogram samples

Electrocardiogram samples are read-only. You can request permission to read the samples using this identifier, but you can’t request authorization to share them. This means you can’t save new electrocardiogram samples to the HealthKit store. To add test data in iOS Simulator, open the Health app and select Browse \> Heart \> Electrocardiograms (ECG) \> Add Data.

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


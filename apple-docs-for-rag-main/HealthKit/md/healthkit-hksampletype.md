

- HealthKit
-  HKSampleType 

Class

# HKSampleType

An abstract superclass for all classes that identify a specific type of sample when working with the HealthKit store.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKSampleType
```

## Overview

The HKSampleType class is an abstract subclass of the HKObjectType class, used to represent data samples. Never instantiate an HKSampleType object directly. Instead, work with one of its concrete subclasses: HKCategoryType, HKCorrelationType, HKQuantityType, or HKWorkoutType classes.

## Topics

### Checking the Duration Restriction

var isMinimumDurationRestricted: Bool

A Boolean value that indicates whether samples of this type have a minimum time interval between the start and end dates.

var minimumAllowedDuration: TimeInterval

The minimum duration if the sample type has a restricted duration.

var isMaximumDurationRestricted: Bool

A Boolean value that indicates whether samples of this type have a maximum time interval between the start and end dates.

var maximumAllowedDuration: TimeInterval

The maximum duration if the sample type has a restricted duration.

### Checking on Recalibrating Estimates

var allowsRecalibrationForEstimates: Bool

A Boolean value that indicates whether HealthKit supports recalibrating the prediction algorithm used to produce estimates for this sample type.

## Relationships

### Inherits From

- HKObjectType

### Inherited By

- HKAudiogramSampleType
- HKCategoryType
- HKClinicalType
- HKCorrelationType
- HKDocumentType
- HKElectrocardiogramType
- HKPrescriptionType
- HKQuantityType
- HKScoredAssessmentType
- HKSeriesType
- HKStateOfMindType
- HKWorkoutType

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


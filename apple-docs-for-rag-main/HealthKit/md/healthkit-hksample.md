

- HealthKit
-  HKSample 

Class

# HKSample

A HealthKit sample represents a piece of data associated with a start and end time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKSample
```

## Mentioned in 

About the HealthKit framework

Saving data to HealthKit

Dividing a HealthKit workout into activities

## Overview

The `HKSample` class is an abstract class. You should never instantiate a `HKSample` object directly. Instead, you always work with one of its concrete subclasses: HKCategorySample, HKQuantitySample, HKCorrelation, or HKWorkout classes.

HealthKit samples are all immutable: You set the sample’s properties when you create it, and they cannot change.

If the sample represents data over a duration, the start time must be earlier than the end time. If the sample represents data at a particular instant, the start and end times can be the same.

## Topics

### Accessing the Sample’s Data

var startDate: Date

The sample’s start date.

var endDate: Date

The sample’s end date.

var hasUndeterminedDuration: Bool

Indicates whether the sample has an unknown duration.

var sampleType: HKSampleType

The sample type.

### Specifying Sort Identifiers

let HKSampleSortIdentifierStartDate: String

A constant for sorting samples based on their start date.

let HKSampleSortIdentifierEndDate: String

A constant for sorting samples based on their end date.

### Specifying Predicate Key Paths

let HKPredicateKeyPathStartDate: String

The key path for accessing the sample’s start date.

let HKPredicateKeyPathEndDate: String

The key path for accessing the sample’s end date.

## Relationships

### Inherits From

- HKObject

### Inherited By

- HKAudiogramSample
- HKCategorySample
- HKClinicalRecord
- HKCorrelation
- HKDocumentSample
- HKElectrocardiogram
- HKQuantitySample
- HKScoredAssessment
- HKSeriesSample
- HKStateOfMind
- HKVerifiableClinicalRecord
- HKVisionPrescription
- HKWorkout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Abstract superclasses

class HKQuantitySample

A sample that represents a quantity, including the value and the units.

class HKObject

A piece of data that can be stored inside the HealthKit store.


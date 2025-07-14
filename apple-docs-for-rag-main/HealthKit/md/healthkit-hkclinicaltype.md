

- HealthKit
-  HKClinicalType 

Class

# HKClinicalType

A type that identifies samples that contain clinical record data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
class HKClinicalType
```

## Topics

### Creating Clinical Types

convenience init(HKClinicalTypeIdentifier)

Creates a clinical type using the provided identifier.

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

class HKClinicalRecord

A sample that stores a clinical record.

static let allergyRecord: HKClinicalTypeIdentifier

A type identifier for records of allergic or intolerant reactions.

static let conditionRecord: HKClinicalTypeIdentifier

A type identifier for records of a condition, problem, diagnosis, or other event.

static let immunizationRecord: HKClinicalTypeIdentifier

A type identifier for records of the current or historical administration of vaccines.

static let labResultRecord: HKClinicalTypeIdentifier

A type identifier for records of lab results.

static let medicationRecord: HKClinicalTypeIdentifier

A type identifier for records of medication.

static let procedureRecord: HKClinicalTypeIdentifier

A type identifier for records of procedures.

static let vitalSignRecord: HKClinicalTypeIdentifier

A type identifier for records of vital signs.

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

class HKWorkoutType

A type that identifies samples that store information about a workout.

class HKObjectType

An abstract superclass with subclasses that identify a specific type of data for the HealthKit store.

class HKSampleType

An abstract superclass for all classes that identify a specific type of sample when working with the HealthKit store.


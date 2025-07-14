

- HealthKit
-  HKObjectType 

Class

# HKObjectType

An abstract superclass with subclasses that identify a specific type of data for the HealthKit store.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class HKObjectType
```

## Mentioned in 

Saving data to HealthKit

About the HealthKit framework

## Overview

The `HKObjectType` class is an abstract class. Don’t instantiate an `HKObjectType` object directly. Instead, instantiate one of the following concrete subclasses:

- HKActivitySummaryType

- HKCategoryType

- HKCorrelationType

- HKCharacteristicType

- HKDocumentType

- HKQuantityType

- HKSeriesType

- HKWorkoutType

The `HKObjectType` class provides a convenience method to create each of these subclasses.

### Work with Object Types

Like many HealthKit classes, HealthKit object types aren’t extensible. Don’t subclass these classes.

Additionally, wherever possible, this class uses a single instance to represent all copies of the same type. For example, if you make two calls to the quantityType(forIdentifier:) method with the same identifier, the system returns the same instance. Reusing object types helps reduce HealthKit’s overall memory usage.

## Topics

### Creating quantity types

class func quantityType(forIdentifier: HKQuantityTypeIdentifier) -> HKQuantityType?

Returns the shared quantity type for the provided identifier.

struct HKQuantityTypeIdentifier

The identifiers that create quantity type objects.

### Creating category types

class func categoryType(forIdentifier: HKCategoryTypeIdentifier) -> HKCategoryType?

Returns the shared category type for the provided identifier.

struct HKCategoryTypeIdentifier

Identifiers for creating category types.

### Creating characteristic types

class func characteristicType(forIdentifier: HKCharacteristicTypeIdentifier) -> HKCharacteristicType?

Returns the shared characteristic type for the provided identifier.

struct HKCharacteristicTypeIdentifier

The identifiers that create characteristic type objects.

### Creating correlation types

class func correlationType(forIdentifier: HKCorrelationTypeIdentifier) -> HKCorrelationType?

Returns the shared correlation type for the provided identifier.

struct HKCorrelationTypeIdentifier

The identifiers that create correlation type objects.

### Creating workout types

class func workoutType() -> HKWorkoutType

Returns the shared HKWorkoutType object.

### Creating activity summary types

class func activitySummaryType() -> HKActivitySummaryType

Returns the shared activity summary type.

### Creating electrocardiogram types

class func electrocardiogramType() -> HKElectrocardiogramType

Returns the shared electrocardiogram type.

### Creating audiogram sample types

class func audiogramSampleType() -> HKAudiogramSampleType

Returns an audiogram sample type.

### Creating vision prescription types

class func visionPrescriptionType() -> HKPrescriptionType

Returns a shared vision prescription type object.

### Creating clinical record types

class func clinicalType(forIdentifier: HKClinicalTypeIdentifier) -> HKClinicalType?

Returns the shared clinical type for the provided identifier.

### Creating series types

class func seriesType(forIdentifier: String) -> HKSeriesType?

Returns the shared series type for the provided identifier.

### Creating document types

class func documentType(forIdentifier: HKDocumentTypeIdentifier) -> HKDocumentType?

Returns the shared document type for the provided identifier.

struct HKDocumentTypeIdentifier

The identifiers for documents.

### Getting property data

var identifier: String

A unique string identifying the HealthKit object type.

func requiresPerObjectAuthorization() -> Bool

Returns a Boolean that indicates whether the data type requires per-object authorization.

### Type Methods

class func stateOfMindType() -> HKStateOfMindType

## Relationships

### Inherits From

- NSObject

### Inherited By

- HKActivitySummaryType
- HKCharacteristicType
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

class HKElectrocardiogramType

A type that identifies samples containing electrocardiogram data.

class HKSeriesType

A type that indicates the data stored in a series sample.

class HKClinicalType

A type that identifies samples that contain clinical record data.

class HKWorkoutType

A type that identifies samples that store information about a workout.

class HKSampleType

An abstract superclass for all classes that identify a specific type of sample when working with the HealthKit store.


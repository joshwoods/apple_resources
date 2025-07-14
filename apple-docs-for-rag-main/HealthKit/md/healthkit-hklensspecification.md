

- HealthKit
-  HKLensSpecification 

Class

# HKLensSpecification

An abstract superclass for lens specifications.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class HKLensSpecification
```

## Overview

Don’t instantiate this class directly. Instead, use one of its concrete subclasses: HKGlassesLensSpecification or HKContactsLensSpecification.

## Topics

### Accessing lens specification data

var sphere: HKQuantity

The correction for farsightedness.

var cylinder: HKQuantity?

Part of the correction for astigmatism that measures the strength of the correction.

var axis: HKQuantity?

Part of the correction for astigmatism that measures the orientation fo the correction.

var addPower: HKQuantity?

The correction for nearsightedness.

## Relationships

### Inherits From

- NSObject

### Inherited By

- HKContactsLensSpecification
- HKGlassesLensSpecification

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Vision prescriptions

class HKVisionPrescription

A sample that stores a vision prescription.

class HKGlassesPrescription

A sample that stores a prescription for glasses.

class HKContactsPrescription

A sample that store a prescription for contacts.

class HKGlassesLensSpecification

An object that contains the glasses prescription data for one eye.

class HKContactsLensSpecification

An object that contains the contacts prescription data for one eye.

class HKVisionPrism

Prescription data for eye alignment.

class HKPrescriptionType

A type that identifies samples that store a prescription.


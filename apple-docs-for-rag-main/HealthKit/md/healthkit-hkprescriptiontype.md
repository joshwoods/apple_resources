

- HealthKit
-  HKPrescriptionType 

Class

# HKPrescriptionType

A type that identifies samples that store a prescription.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class HKPrescriptionType
```

## Overview

The HKPrescriptionType class is a concrete subclass of the HKSampleType class. To create a vision prescription type instances, use the visionPrescriptionType() convenience method.

Use this data type to request permission to save vision prescriptions to the HealthKit store.

```
// Create the prescription data type.
let visionPrescriptionType = HKObjectType.visionPrescriptionType()

// Request authorization to save vision prescription samples.
store.requestAuthorization(toShare: [visionPrescriptionType],
                           read: []) { success, error in
    if let error {
        // Handle errors here.
        fatalError("*** An error occurred while requesting permission: \(error.localizedDescription) ***")
    }
}
```

Note

Important Vision prescription samples require per-object authorization. Requesting authorization to read these samples using requestAuthorization(toShare:read:) fails with an error. Instead, use requestPerObjectReadAuthorization(for:predicate:completion:) to request authorization before querying for samples.

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

class HKLensSpecification

An abstract superclass for lens specifications.

class HKVisionPrism

Prescription data for eye alignment.


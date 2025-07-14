

- HealthKit
-  HKVisionPrescriptionType 

Enumeration

# HKVisionPrescriptionType

The type of vision prescription, for example a prescription for glasses or for contacts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
enum HKVisionPrescriptionType
```

## Topics

### Prescription types

case glasses

A prescription for glasses.

case contacts

A prescription for contacts.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing the prescription data

var prescriptionType: HKVisionPrescriptionType

The type of vision prescription.

var dateIssued: Date

The date when the doctor issued the prescription.

var expirationDate: Date?

The date when the prescription expires.


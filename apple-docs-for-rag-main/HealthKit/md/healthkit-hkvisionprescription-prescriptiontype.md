

- HealthKit
- HKVisionPrescription
-  prescriptionType 

Instance Property

# prescriptionType

The type of vision prescription.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var prescriptionType: HKVisionPrescriptionType { get }
```

## Discussion

This property contains a value that indicates the type of prescription. For a list of possible values, see HKVisionPrescriptionType.

## See Also

### Related Documentation

class HKGlassesPrescription

A sample that stores a prescription for glasses.

class HKContactsPrescription

A sample that store a prescription for contacts.

### Accessing the prescription data

enum HKVisionPrescriptionType

The type of vision prescription, for example a prescription for glasses or for contacts.

var dateIssued: Date

The date when the doctor issued the prescription.

var expirationDate: Date?

The date when the prescription expires.


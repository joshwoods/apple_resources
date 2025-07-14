

- HealthKit
- HKVisionPrescription
-  dateIssued 

Instance Property

# dateIssued

The date when the doctor issued the prescription.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var dateIssued: Date { get }
```

## See Also

### Accessing the prescription data

var prescriptionType: HKVisionPrescriptionType

The type of vision prescription.

enum HKVisionPrescriptionType

The type of vision prescription, for example a prescription for glasses or for contacts.

var expirationDate: Date?

The date when the prescription expires.


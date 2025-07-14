

- HealthKit
- HKClinicalRecord
-  clinicalType 

Instance Property

# clinicalType

An identifier that indicates the type of record, such as an allergic reaction, a lab result, or a medical procedure.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
@NSCopying
var clinicalType: HKClinicalType { get }
```

## See Also

### Accessing Clinical Record Data

var displayName: String

The primary display name as shown in the Health app.

var fhirResource: HKFHIRResource?

The Fast Healthcare Interoperability Resources (FHIR) data for this record.


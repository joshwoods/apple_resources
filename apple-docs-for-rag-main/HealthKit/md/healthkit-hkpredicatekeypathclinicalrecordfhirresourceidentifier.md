

- HealthKit
-  HKPredicateKeyPathClinicalRecordFHIRResourceIdentifier 

Global Variable

# HKPredicateKeyPathClinicalRecordFHIRResourceIdentifier

The key path for accessing the clinical record’s Fast Healthcare Interoperability Resources (FHIR) identifier.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
let HKPredicateKeyPathClinicalRecordFHIRResourceIdentifier: String
```

## Discussion

The FHIR resource identifier is only unique for a particular resource type from a given source. To uniquely identify a FHIR resource, you must compare the identifier, the resource type, and the source.

## See Also

### Clinical record keys

let HKPredicateKeyPathClinicalRecordFHIRResourceType: String

The key path for accessing the resource type of a Fast Healthcare Interoperability Resources (FHIR) record.


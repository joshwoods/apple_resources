

- HealthKit
- HKQuery
-  predicateForClinicalRecords(withFHIRResourceType:) 

Type Method

# predicateForClinicalRecords(withFHIRResourceType:)

Returns a predicate for a specific FHIR type.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
class func predicateForClinicalRecords(withFHIRResourceType resourceType: HKFHIRResourceType) -> NSPredicate
```

## Mentioned in 

Accessing Health Records

## See Also

### Creating clinical record predicates

class func predicateForClinicalRecords(from: HKSource, fhirResourceType: HKFHIRResourceType, identifier: String) -> NSPredicate

Returns a predicate for a specific FHIR resource.

class func predicateForVerifiableClinicalRecords(withRelevantDateWithin: DateInterval) -> NSPredicate

Returns a predicate that finds verifiable health records with a relevant date within the specified range.


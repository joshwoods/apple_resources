

- HealthKit
- HKQuery
-  predicateForVerifiableClinicalRecords(withRelevantDateWithin:) 

Type Method

# predicateForVerifiableClinicalRecords(withRelevantDateWithin:)

Returns a predicate that finds verifiable health records with a relevant date within the specified range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
class func predicateForVerifiableClinicalRecords(withRelevantDateWithin dateInterval: DateInterval) -> NSPredicate
```

## Parameters 

`dateInterval`  

The start and end date for the predicate.

## Discussion

The resulting predicate matches HKVerifiableClinicalRecord instances that have a relevantDate property within the specified date interval.

## See Also

### Creating clinical record predicates

class func predicateForClinicalRecords(from: HKSource, fhirResourceType: HKFHIRResourceType, identifier: String) -> NSPredicate

Returns a predicate for a specific FHIR resource.

class func predicateForClinicalRecords(withFHIRResourceType: HKFHIRResourceType) -> NSPredicate

Returns a predicate for a specific FHIR type.


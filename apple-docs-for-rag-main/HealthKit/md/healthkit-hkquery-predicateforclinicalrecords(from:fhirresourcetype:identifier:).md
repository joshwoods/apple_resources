

- HealthKit
- HKQuery
-  predicateForClinicalRecords(from:fhirResourceType:identifier:) 

Type Method

# predicateForClinicalRecords(from:fhirResourceType:identifier:)

Returns a predicate for a specific FHIR resource.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+

``` source
class func predicateForClinicalRecords(
    from source: HKSource,
    fhirResourceType resourceType: HKFHIRResourceType,
    identifier: String
) -> NSPredicate
```

## Mentioned in 

Accessing Health Records

## Discussion

The FHIR resource identifier is only unique for a particular resource type from a given source. To uniquely identify a FHIR resource, you must compare the identifier, the resource type, and the source.

## See Also

### Creating clinical record predicates

class func predicateForClinicalRecords(withFHIRResourceType: HKFHIRResourceType) -> NSPredicate

Returns a predicate for a specific FHIR type.

class func predicateForVerifiableClinicalRecords(withRelevantDateWithin: DateInterval) -> NSPredicate

Returns a predicate that finds verifiable health records with a relevant date within the specified range.


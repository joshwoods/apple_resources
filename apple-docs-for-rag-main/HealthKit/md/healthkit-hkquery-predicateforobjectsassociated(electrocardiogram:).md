

- HealthKit
- HKQuery
-  predicateForObjectsAssociated(electrocardiogram:) 

Type Method

# predicateForObjectsAssociated(electrocardiogram:)

Returns a predicate that matches symptom samples associated with the specified electrocardiogram.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+watchOS 7.0+

``` source
class func predicateForObjectsAssociated(electrocardiogram: HKElectrocardiogram) -> NSPredicate
```

## Parameters 

`electrocardiogram`  

The target electrocardiogram.

## Return Value

A predicate that matches symptom samples associated with the specified electrocardiogram.

## Discussion

If the HKElectrocardiogram sample’s symptomsStatus property is HKElectrocardiogram.SymptomsStatus.present, you can query for symptom samples associated with the electrocardiogram. See Symptom Type Identifiers for a complete list of symptom types.

## See Also

### Creating electrocardiogram predicates

class func predicateForElectrocardiograms(classification: HKElectrocardiogram.Classification) -> NSPredicate

Returns a predicate that matches electrocardiogram samples with the specified classification.

class func predicateForElectrocardiograms(symptomsStatus: HKElectrocardiogram.SymptomsStatus) -> NSPredicate

Returns a predicate that matches electrocardiogram samples with the specified symptom status.


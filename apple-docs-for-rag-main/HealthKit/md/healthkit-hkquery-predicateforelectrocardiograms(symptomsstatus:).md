

- HealthKit
- HKQuery
-  predicateForElectrocardiograms(symptomsStatus:) 

Type Method

# predicateForElectrocardiograms(symptomsStatus:)

Returns a predicate that matches electrocardiogram samples with the specified symptom status.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class func predicateForElectrocardiograms(symptomsStatus: HKElectrocardiogram.SymptomsStatus) -> NSPredicate
```

## Parameters 

`symptomsStatus`  

The target symptom status.

## Return Value

A predicate that matches electrocardiogram samples with the specified symptom status.

## Discussion

Use this convenience method to create a predicate that matches electrocardiogram samples with the specified symptom status. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

```
let forSymptomStatus = HKQuery.predicateForElectrocardiograms(symptomsStatus: .present)

let status = HKElectrocardiogram.SymptomsStatus.present.rawValue

let explicitForSymptomStatus = NSPredicate(format: "%K == %d", HKPredicateKeyPathECGSymptomsStatus, status)
```

## See Also

### Related Documentation

let HKPredicateKeyPathECGSymptomsStatus: String

The key path for the sample’s symptom status.

### Creating electrocardiogram predicates

class func predicateForElectrocardiograms(classification: HKElectrocardiogram.Classification) -> NSPredicate

Returns a predicate that matches electrocardiogram samples with the specified classification.

class func predicateForObjectsAssociated(electrocardiogram: HKElectrocardiogram) -> NSPredicate

Returns a predicate that matches symptom samples associated with the specified electrocardiogram.


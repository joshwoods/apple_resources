

- HealthKit
- HKQuery
-  predicateForElectrocardiograms(classification:) 

Type Method

# predicateForElectrocardiograms(classification:)

Returns a predicate that matches electrocardiogram samples with the specified classification.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class func predicateForElectrocardiograms(classification: HKElectrocardiogram.Classification) -> NSPredicate
```

## Parameters 

`classification`  

The target classification.

## Return Value

A predicate that matches electrocardiogram samples with the specified classification.

## Discussion

Use this convenience method to create a predicate that matches electrocardiogram samples with the specified classification. The following sample uses both the convenience method and a predicate format string to create equivalent predicates.

```
let forClassification = HKQuery.predicateForElectrocardiograms(classification: .atrialFibrillation)

let classification = HKElectrocardiogram.Classification.atrialFibrillation.rawValue

let explicitForClassification = NSPredicate(format: "%K == %d", HKPredicateKeyPathECGClassification, classification)
```

## See Also

### Related Documentation

let HKPredicateKeyPathECGClassification: String

The key path for the sample’s classification.

### Creating electrocardiogram predicates

class func predicateForElectrocardiograms(symptomsStatus: HKElectrocardiogram.SymptomsStatus) -> NSPredicate

Returns a predicate that matches electrocardiogram samples with the specified symptom status.

class func predicateForObjectsAssociated(electrocardiogram: HKElectrocardiogram) -> NSPredicate

Returns a predicate that matches symptom samples associated with the specified electrocardiogram.

